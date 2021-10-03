
This document describes how individual tasks are approved, tested, merged, and deployed.

* Our process is inspired by Raycast & their [no code review](https://www.raycast.com/blog/no-code-reviews-by-default/) process (with some modifications). 
* We use [Linear](https://linear.app) for project management. We use [roadmaps](https://linear.app/method/roadmap) for planning, [fibonacci numbers](https://www.mathsisfun.com/numbers/fibonacci-sequence.html) for complexity rating and cycles for momentum tracking. 

# 1. 🌳 Git Branching

### 1.1 🕊 Code Flow Branches
* `master`/`main`: production ready, stable code.
* `development`: pre-production code that has been developed and is ready for QA and when tested will be merged and deployed to production.

### 1.2 🔖 Temporary Branches
Disposable branches that can be created for proposed changes. 

Format: `#{user}/#{identifier}-#{title}`

* User: The user who is introducting the change. 
* Ticket ID: Linear's unique ID for the ticket that describes the task that this branch addresses.
* Title: Short readable title for the branch with words separated by `-`.

e.g. `daniel/ISQ-77-fix-tests-on-github-actions`


# 2. 📦 Issue Type

### 2.1 ☑️ Tasks - Updates, New Features, Improvements
1. Tasks ([tasks not user stories](https://linear.app/method/write-tasks-not-user-stories)) are created in Linear. The tasks that prioritized are planning into a cycle.
2. If this task is urgent, it is prioritized in the current cycle.
3. Task is picked up, branch out from `development` for development.

## 2.2 🐞 Expedited Bugs / Hot Fix
1. Bug report is analyzed to be prioritized immediately or planned for a later cycle. Prioritization is based on the impact and criticality of the issue.  
2. Expedited bugs are branched out from `master`/`main`.

# 3. 👩‍💻 Development 
1. After development, add any automated testing required and manually test features with all possible edge cases.
2. Ensure all automated tests pass - including Rubocop and any styling changes to be done. 
3. Create a PR back to the same branch where you branched off from.
4. Add all the details required to create the PR - instructions in the PR template. 

# 4. ✅ Individual Task Testing & Merge
1. Test your individual task in isolation locally. Ensure all automated tests pass.
2. You can optionally request someone else from the team to review your work.
3. Once you are happy with your work, you can merge your PR into `development`. 

# 5. 🏁 Deploy Urgency

### 5.1. 🗓 Testing & Planned Release
1. Create a deploy PR from `development` to `master`/`main`. 
2. Go through each PR that were merged and for each:
3. In the deploy PR add a list of features that have been merged into it with reference to each individual PR. 
4. Copy over the post-deploy notes and aggregate it into the deploy branch. 
5. Run automated testing and ensure all tests still pass. If not, tests need to be fixed manually - loop each developer responsible for that part of the change.
6. Deploy to the staging server and copy over the production database. Run post-deploy scripts on the staging server. 
7. Test everything together on the staging server. If there are any issues, loop in developers as required to fix the code they introduced. 
8. Deploy to production server & action post-deploy actions. 
9. Quick test on the production server. 
10. Merge deploy branch into `master`/`main` & publish a release tag on GitHub. 

### 5.2 🛠 Expedited Bug / Hot Fix Deploy
1. Replicate the issue, fix & test locally.
2. PR is made back into `master`/`main` directly.
3. Merge the PR and deploy to production. 
4. Verify issue has also been resolved on production. Then mark the issue as resolved in our error tracking software. 
5. Communicate back to the reporter of the bug & ask for verification on their end also. 

# 6. 🏷 Creating GitHub Release Tag
1. Draft a new release. 
2. Title with the main highlight. 
3. Description with a list of tasks that were merged - automated with the release drafter task.
4. Tag version number format: `[Major].[Minor].[Patch]` (https://semver.org)
