
# Local System Setup [macOS]

| Emoji | Key |
|--|--|
| :heavy_dollar_sign: | Optional paid software. |
| 💳 | Paid by Identity Square. |
| 🎟 | Request Invite to join team. |


## Initial Setup  ☁️

1. Company Email 💳🎟
2. [Setup Mac with your Apple account](https://support.apple.com/en-us/HT204053)
3. [Enable FindMyMac](https://support.apple.com/en-ie/guide/findmy-mac/fmm53101237/mac)
4. [Hardware encryption with backup key stored in iCloud](https://support.apple.com/en-ie/guide/mac-help/mh11785/mac)
5. Device Endpoint Management 💳🎟

## General Apps 🌳
|Name|Details|
|--|--|
|[Safari](https://www.apple.com/safari/)|Fastest, privacy centred & most power efficient browser on macOS.| 
|[RayCast](https://raycast.com)| Powerful alternative to Spotlight.|


## Terminal :computer:

:point_right: [Follow this tutorial](https://towardsdatascience.com/the-ultimate-guide-to-your-terminal-makeover-e11f9b87ac99) selecting what you want to install. 

We install the following:

|Name|Details|
|--|--|
|[Homebrew](https://brew.sh)|macOS package manager.|
|[iTerm2](https://iterm2.com)|Native terminal replacement that allows you do much more.| 
|[Zsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)|Command line shell.|
|[Oh-My-Zsh](https://github.com/ohmyzsh/ohmyzsh)|Allows you add cool plugins and themes to zsh.|


### Customising your terminal
After you set up Oh-My-Zsh, you will have to edit the hidden file './zshrc' to change themes and add useful plugins. Open in through your terminal to find and edit it. 
```
open ~./zshrc
```
#### :rainbow: Theme
Our preferred theme to add to your './zshrc' file.:
```
ZSH_THEME="powerlevel10k/powerlevel10k"
```
Then close and reopen iTerm. You will get prompts (like [this](https://github.com/romkatv/powerlevel10k#configuration-wizard)). Simply choose your preferences.

#### :electric_plug:  Plugins
These are the plugins to install. Before you put them in, check that you have the prerequisites in the [docs](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/).

* `git`
* `Ruby`
* `Rails`
* `autojump`
* `zsh-autosuggestions`

```
plugins=(git rails autojump ruby)
```
## Development Environment 👾

|Name|Details
|--|--|
|[Ruby](https://www.ruby-lang.org/en/downloads/)|Install Ruby versions needed.|
|[RVM](https://www.driftingruby.com/episodes/a-rubyist-s-apple-m1-review)/[rbenv](https://github.com/rbenv/rbenv)| Ruby version manager.|
|[Redis](https://gist.github.com/tomysmile/1b8a321e7c58499ef9f9441b2faa0aa8)|Used for cache, jobs queue.|
|[Postgres](https://postgresapp.com)|Our primary SQL database.|

## Programming tools  🛠
|Name|Details|
|--|--|
|[Github Desktop](https://desktop.github.com)|Git GUI.| 
|[Postico](https://eggerapps.at/postico/) |GUI for Postgres DB.|
|[Chrome](https://www.google.com/intl/en/chrome/)| Sometimes Chrome is better for JS debugging. |

## Code Editor 👨‍💻
Our preferred code editors: 

1. [Atom](https://atom.io)
2. [SublimeText ](https://www.sublimetext.com) :heavy_dollar_sign:
3. [VSCode](https://code.visualstudio.com)

#### :electric_plug: Plugins

* [Tabnine](https://www.tabnine.com/install) - An AI tool that predicts what you're going to type.
* [Rubocop autocorrect](https://atom.io/packages/rubocop-auto-correct) - A code analyser and format checker to write better Ruby code.
* Customise with your own code editor themes & other plugins.

## Team Communication 💬
|Name|Details|
|--|--|
|[Slack](https://slack.com/intl/en-ie/) 💳🎟 |Our preferred way quickly communicate & ask questions.| 
|[Apple calendar](https://apps.apple.com/us/app/calendar/id1108185179)/ [Fantastical](https://apps.apple.com/us/app/fantastical-calendar-tasks/id718043190) :heavy_dollar_sign: | Setup to get notified of cal invites, events & any event updates.|
|[Apple Mail](https://apps.apple.com/us/app/mail/id1108187098)/[Superhuman](https://superhuman.com) :heavy_dollar_sign:| Email notifications |
|[Loom](https://www.loom.com/)|Record and share quick screencasts.|
|[Around](https://www.around.co) 🎟| Less-official feeling team calls to avoid 'Zoom fatigue'. |
|[Zoom](https://zoom.us)|For external meetings.|


## Organisation  :nerd_face:
|Name|Details|
|--|--|
|[Apple notes](https://support.apple.com/en-ie/HT205773)/[Bear](https://bear.app) :heavy_dollar_sign:|To jot down quick notes.| 
|[Apple Reminders](https://support.apple.com/en-ie/HT205890)|For your personal tasks that can't be tracked on our project management tool. E.g. emails to send, to ring someone, etc.|
|[1Password](https://1password.com) 💳🎟| Create, store strong passwords and access shared secrets. Request invite to team. |
|[Swish](https://highlyopinionated.co/swish/) :heavy_dollar_sign:|Control windows using gestures.|
|[CharlieHR](http://identitysquare.charliehr.com) 💳🎟| HR software to book days-off and performance reviews. |

## Online Tools  🛠

|Name|Details|
|--|--|
|[Dropbox Paper](https://www.dropbox.com/paper)|We use this for quickly scoping out technical documents. A free flow sheet for adding notes, embedding videos, images, code, etc.|
|[Figma](https://www.figma.com)|A wire framing tool for designing apps and mockups.|
|[Miro](https://www.miro.com)|Ideas planning and collaboration sessions.|
|[Jira](https://www.atlassian.com/software/jira)/[Linear](https://linear.app) 💳🎟|Helps streamline software projects, sprints and tasks.|
|[Github](https://www.github.com) 🎟|Our central hub for all our code.|
|[Google Drive](https://drive.google.com) |Shared docs, slides and sheets.| 


## Mobile Apps  :iphone:
* Calendar App / [Fantastical ](https://apps.apple.com/us/app/fantastical-calendar-tasks/id718043190) :heavy_dollar_sign:
* Email App
* Apple Reminders
* [Slack](https://apps.apple.com/us/app/slack/id618783545)
* [Around](https://apps.apple.com/ie/app/around/id1558224935)
* [Zoom](https://apps.apple.com/ie/app/zoom-cloud-meetings/id546505307)
*  [1Password](https://apps.apple.com/app/1password-password-manager/id568903335) 💳🎟

## Keyboard Shortcuts to Memorize & Use :cowboy_hat_face:
|Name|Command|
|--|--|
|Copy|`⌘` + `c`|
|Cut|`⌘` + `x`|
|Paste|`⌘` + `v`|
|Spotlight/RayCast - open and switch apps, search, etc.| `⌘` + `space`| 
|Switch applications|`⌘` + `tab`|
|Screenshot selection|`⌘` + `shift` + `4` |
|Screenshot full screen|`⌘` + `shift` + `3` |
|Delete line|`⌘` + `delete`|
|Delete last word|`option` + `delete`|
|Show hidden files on finder|`⌘` + `shift` + `.`|
|Search & switch files quickly in code editor|`⌘` + `p`|
