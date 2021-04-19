
This document describes how individual tasks are approved, tested, merged, and deployed.

# 1. 🌳 Git Branching

### 1.1 🕊 Code Flow Branches
* `master`/`main`: production ready, stable code.
* `staging`: pre-production testing with code that is ready to be deployed to production.
* `development`: new code that has been developed and is ready for QA and to be send live in the next deploy. 

### 1.2 🔖 Temporary Branches
Disposable branches that can be created for proposed changes. 

Format: `#{type}/#{ticket-id}_#{title}`

* Type: `feature`, `bugfix`, `hotfix`, `experimental`
* Ticket ID: Jira, GitHub Issues or other task management tool's unique ID for the ticket that describes the task that this branch addresses.
* Title: Short readable title for the branch with words separated by `-`.

e.g. `feature/JIRA-1234_support-dark-theme`


# 2. 📦 Issue Type

### 2.1 ☑️ Tasks - Updates, New Features, Improvements
1. Tasks are scoped out with all the details. The task is prioritized and planning into a sprint.
2. If this task is urgent, it is prioritized in the current week's work while deprioritizing something else.
3. Task is picked up, branch out from `development` for development. (Or the main feature branch if it's a sub-task).

## 2.2 🐞 Expedited Bugs / Hot Fix
1. Bug report is analyzed to be prioritized immediately or planned for a later sprint. Prioritization is based on the impact and criticality of the issue.  
2. Expedited bugs are branched out from `master`/`main`.

# 3. 👩‍💻 Development 
1. After development, add any automated testing required and manually test features with all possible edge cases.
2. Ensure all automated tests pass - including Rubocop and any styling changes to be done. 
3. Create a PR back to the same branch where you branched off from.
4. Create & deploy to Heroku review environment (automated) and copy production DB into the new environment. 
5. Add all the details required to create the PR - instructions in the PR template. 

# 4. ✅ Individual Task Testing & Approval
1. Test the individual task in isolation in the test environment. 
2. Code is reviewed by others. 
3. Feedback is addressed and the review process restarts.
4. Once feedback is approved by all reviewers, the task is tagged as approved and PR is merged into `development`. 

# 5. 🏁 Deploy Urgency

### 5.1. 🗓 Planned Release
1. Merge `development` into `staging`.
2. Create a deploy PR from `staging` to `master`/`main`. 
3. Go through each PR that are approved and for each:
4. In the deploy PR add a list of features that have been merged into it with reference to each individual PR. 
5. Copy over the post-deploy notes and aggregate it into the deploy branch. 
6. Run automated testing and ensure all tests pass. If not, tests need to be fixed manually - loop each developer responsible for that part of the change.
7. Deploy to the staging server and copy over the production database. Run post-deploy scripts on the staging server. 
8. Test everything together on the staging server. 
9. Deploy to production server & do post-deploy actions. 
10. Quick test on the production server. 
11. Merge deploy branch into `master`/`main`, draft & publish a release tag on GitHub. 
12. Create a release on Jira to capture all the tasks that went live with the deployment / or complete sprint in any other task management tool.

### 5.2 🛠 Expedited Bug / Hot Fix Deploy
1. PR is back into `master`/`main` directly. 
2. Merge the PR and deploy to production. 
3. Verify issue has been resolved on production. 
4. Communicate back to the reporter of the bug & ask for verification on their end also. 

# 6. 🏷 Creating GitHub Release Tag
1. Draft a new release. 
2. Title with the main highlight. 
3. Description with a list of tasks that were merged - automated with the release drafter task.
4. Tag version number format: `[Major].[Minor].[Patch]` (https://semver.org)
