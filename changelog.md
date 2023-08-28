# Changelog

 ## Sophie v2.2
## Released 20th November 2020

- Added ability to save btnnotes like `[Button name](#notename)`
- Implement regex support in fiters
- Added bot add button in the /start menu
- Fixed parsing non-existent buttons in notes
- Show a link to return to the chat after passing a welcome security
- Fixed sending welcome to user's pm if welcomes was disabled and welcomesecurity is enabled
- Admins now able to access disabled commands
- Added antiflood module
- Alias /fbanstat to /fcheck
- Alias /antiflood to /flood
- Beauty fixes for /addfilter
- Added ability to unpin all messages via /unpin all
- Added ability to pin messages in PM
- Restricted ability to create new Federations by anon admins
- Added ability to set a custom reason for a half of filters actions
- /admins now won't show anon admins
- Added /defilters command to remove all filters of a chat
- Added ability to use /connect command for anon admins
- Improved perfomance for Federations module
- Improved perfomance for Connections module
- From now /promote will promote new admins without `'Adding new admins'` permission
- Added support for customized join expiration time for greetings
- Fixes for anon admins
- Fixed some typos
- Fixes for connections
- Fixes for duplications of fbanning
- Fixes for importing for greeting
- Many other improvments and fixes

**Internal changes:**

- Support for custom BotAPI Server
- Add /logs ability for OPs

 
## Sophie v2.1
  ## Released 13th June 2020

- /fsetlog now supports channels
- Added /fcheck command to check if the user was banned in other Federations. Using it on yourself will result in a list of Federations you are banned in. Sophie respects your privacy and won't show banned Federation names to unknown people.
- Added /privatenotes commands which replaces /notes command with `'See notes in PM',` this will redirect users to Sophie's PM instead of using notes in your chats.
- Notes now support `'-'` in the name and it won't cause any problems.
- From now 'Reply' action in filters are supports buttons, links, and media.
- Improved buttonrules - A rules button.
- Fixed `"WelcomeSecurity button does not appear in some Telegram clients and big chats".`
- Fixed connecting with chat username
- From now /help is can be disabled
- Fixed some bugs in /promote command.

## Sophie v2.1.4
## Released 14th June 2020

- Fixes the NoneType handler column if no argument provided for /addfilter.

## Sophie v2.1.5
## Released 17th June 2020

- Improvements in /fcheck command
- Fed logs now include user_id and Fed admin
- The Welcome Security button is now inline and should be fixed on weird Telegram clients and big chats
- Fixes under the /disconnect command
- More small bug fixes and improvements


## Sophie v2.1.6
## Released 18th June 2020

- Small fixes under connections and warns.

## Sophie v2.1.7
## Released 20th June 2020

- Fixed Un-FedBanning errors with enabled Fed logs in some cases
- /clear now will tell about nonexistent note name
- Also from now /fadmins and /admins won't tag admins.

## Sophie v2.1.8
## Released 21th June 2020

- Fixed `"raw"` argument in the /get command
- Fixed `"_"` in the note name now won't cause error in the btnnnote
- Now she will give a warning if admin title contains emoji and won't crash.

### Sophie v2.1.9
Released 24th June 2020

- Now she knows Turkish 🇹🇷.
- Spanish 🇪🇸 language was updated
- Fixed some bugs also like supporting escaping HTML from admin titles in /promote
- Fixes in error handling.

## Sophie v2.1.10
## Released 25th June 2020

- Minor fixes with strings
- Added catching few more exceptions for welcome security
- Cleaning notes now won't remove last note message if new one wasn't sent for some reasons like not found.

## Sophie v2.1.11
## Released 26th June 2020

- Improved speed of the /fimport command

## Sophie v2.1.12
## Released 6th July 2020

- Fixed small errors like missing Exceptions and fixed updating very old notes.

## Sophie v2.1.13
## Released 16th July 2020

- Fixed crashing which came after setting new filters in some cases.

## Sophie v2.1.14
## Released 24th July 2020

- Prevent to saving filters with None type, it won't cause crashes anymore
- Reports tagging now will have zero width space
- Fixed under parsing times for commands with `'t'` prefix
- Added catching more exception in the restriction module
- Fixed wrong string name in the /search command

**Also added new stuff:**

- Ability to change fed ban reason by fbanning already banned user
- Added Czech language
- Improved Russian translation

## Sophie v2.1.16
## Released 3th August 2020

- Fixed notes mention on reply, no Sophie will mention replied user
- Fixed showing previews for notes
- Fixed crashing if the reason wasn't given at first place in the fbanning command
- Removed undocumented welcomestrict future which we forgot to remove after merging staging to v2.1 branch.
- Improved delete button if using with filters
- Added missed exception in notes which will fix crashing if a user is blocked
- From now /connect (chat username) is case-insensitive
- From now Sophie won't mute new bots added by admins
- From now Sophie won't delete user's unmute button in case if other muted user is clicked on it
- From now muted users via /mute can't bypass it by using welcomesecurity button
- From now /warns command won't tag admins
- Improved code style

## Sophie v2.1.17
## Released 17th August 2020

- Fixed notes reply mention if getting notes via hashtag
- Small bug fixes under greetings
- Ability to remove fed ban reason
- Fixed welcome security expiration
- Minor strings changes
- Fixed saving notes if newline is right after note name

## Sophie v2.1.18
## Released 1th September 2020

- Removed /runs command
- Temporary removed Russian's federations translate until it will be re-translated
- /cleannotes was improved and now supports cleaning more notes commands
- From now you can manage your federation directly in the PM without connecting to the chats
- Fixed escaping quotes
- Fixed error after adding many users per one time
- Many fixes under /fimport command
- Minor other fixes under federations and filters

## Sophie v2.1.19
## Released 17th September 2020

- Disallow to change own admin title
- Feds: fixes with parsing Federation names
- Feds: alias /fedinfo to /finfo
- Feds: /finfo won't tag federation creator from now
- Notes: minor parsing fixes
- Updated Czech language 🇨🇿

## Sophie v2.1.20
## Released 7th October 2020

- Fixed parsing note aliases
- Fixed formatting chat title in the /welcomemute string
- Bunch of other fixed under notes which include more errors handeling
- From now you could reply any message with '/saverules' to save it
- Minor feds fixes and improvements
- Implemented initial anonymous admins support
- Added Arabic 🇮🇶, French 🇫🇷 , and updated Spanish 🇪🇸 with Brazilian 🇧🇷 language.

## Sophie v2.0
## Released 13th May 2020

### General changes
- Now Sophie checks admin rights to make sure the user has rights to perform the action. For example, if the user doesn't have permission to ban users, he/she can't use /ban command
- Sophie's help moved to the https://wiki.sophiebot.gq, help module is removed
- Sudo users were removed and converted to operators
- Global bans were removed
- Improved perfomance a lot
- Fixed English localization
- Fixed issue when the command can be recognized not on the first line of the message
- Added Imports/exports feature
- Added stickers module
- Added locks module

### Notes
- Support saving inline URL buttons from other bots
- Support resaving inline callblacks buttons from Sophie's messages
- Encryption method was changed to default MongoDB's one, it makes the decryption process faster and simpler
- Improved support for saving already formatted messages (Telegram X issue fixed)
- Underline and strikethrough now supported
- Implemented cashtags instead of old note settings, for example, instead of `[format:html]` you have to `%PARSEMODE_HTML` old parsing settings left for backward compatibility
- Implemented new notes variables - `{date}, {time}`
- Forbidden to save blank notes
- Implemented /clearall command.
- Implemented /search command to do a text search query in notes
- Implemented sorting by note name in /notes command feature
- Implemented notes aliases features
- Implemented way to remove many notes by one command.
- From now buttonnote in chats will redirect in Sophie's PM
- From now clicking on buttonnote in Sophie's PM will edit message instead of sending new
- Minor strings changes
- `'buttonnote'` now will redirect in Sophie's PM instead of trying PM you first
- And many other notes changes and bug fixes

### Federations

- Implemented federation subscriptions
- Implemented federation logs
- Sophie now can fban users which she couldn't get (works only with user ID as argument)
- Implemented /fadmins command
- Implemented /fimport and /fexport command
- Implemented /freneame command
- Added timestamp for every federation ban
- Fixed bug when reason text sometimes splitted to reasontext

### Warnings
- /delwarns now aliased to /resetwarns
- Many improvements and fixes

### Misc
- /stats are now allowed only for operators
- /runs can be disabled for now


### Restrictions
- Added silent commands for bans, mutes and kicking, like /skick or /sban
- Now after kicking or banning Sophie will delete 'Sophie removed X' service message
- Removed /kickme command

### Greetings
- Module was fully rewrited
- /setwelcome now doesn't require note with welcome message in
- Now to disable welcome you have to use /setwelcome off
- Updated welcome security: added security levels (button, math, captcha).
- Added security note with which user will be propmted to validate his status in bot's PM.
- Now if welcome security is enabled, Sophie won't send welcome message in chat, but she will send in user's PM after they proved them as human.
- Added /welcomemute feature

### Warnings
- Implemented /warnaction
- Many improvements and fixes

### Filters
- Now /addfilter gets keyword by argument instead of asking it by state
- Filters now fully modular and support inegration by other modules
- Filters now works in pm if user is connected by /connect feature
- Many improvements and fixes

### Users
- Implemented /admincache command, which updates admins cache
- From now /adminlist won't clear admins cache

### Languages
- Many improvements and fixes

### Connections
- Many improvements and fixes
- Added /allowusersconnect to disallow users to connect to chat (admins will be able to connect to the chat)
- If user hasn't started dialog with Sophie, but connected to the chat directly, after starting bot Sophie will reply with the `'connected successfully'` message

### Errors reporting and crashlytics
- Sophie is now using sentry.io as crashlytics storage
- Removed the raw crash files feature
- Sophie won't spam with same error message anymore

### Code changes
- Mainly we focus to support GNU/Linux OS or Docker, but Sophie may work on other OSs too.
- Bot config file changed to YAML
- Removed support of Telethon as commands register
- Sophie is now fully modular, modules ain't depending on each other
- Migrated from MongoDB Pymongo to MongoDB Motor
- Components were removed
- Dockerfile base image was changed to an Alpine instead of Ubuntu
- Translations were converted to YAML files instead of JSON
- Logging changed to a loguru library

**And tons of other edits and fixes**

### For selfhosting
 - From now we are focused on Docker image, so you can easely run it by Docker/podman
 - Docker image can be downloaded and runned from GitLab, no need to build Docker image manually anymore.
 - GitLab auto CI updates docker images with every commit, so docker image will be always latest
 - In v2 introduced database structure migrator, this inbuilt tools will automatically update database for new versions.
 - From now logs will be saved in Logs/ directory

## Sophie v2.0.5
## Released 25th May 2020

- Improved sub-Federations
- Improved support of importing fed bans from other bots
- Improved speed of importing/exporting fed bans
- From now /fexport will export bans in csv format.

## Sophie v2.0.6
## Released 25th May 2020

**Make your chats more clean with Sophie 2.0.6.**

- Implemented /cleannotes which will remove old notes messages (like /cleanwelcome works)
- Implemented /sfban: Silent federation ban which will purge messages after fban will be done
