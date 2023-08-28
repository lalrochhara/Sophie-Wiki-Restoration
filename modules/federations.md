Well, basically there are two reasons to use Federations:

You have many chats and want to ban users in all of them with one command
You want to subscribe to any existing anti-spam federations to have your chat(s) protected
In both cases Sophie will help you!

## Avaible commands
**Arguments types legend:**

(): required argument
(user): required but you can reply on any user's message instead
(file): required file, if file isn't provided you will be entered in file state, this means Sophie will wait file message from you. Type /cancel to leave from it.
(? ): additional argument`

## Only Federation owner
- /fnew (name) or /newfed (name): Creates a new federation
- /frename (?Fed ID) (new name): Renames your federation
- /fdel (?Fed ID) or /delfed (?Fed ID): Removes your federation
- /fpromote (user) (?Fed ID): Promotes a user to the your federation
- /fdemote (user) (?Fed ID): Demotes a user from the your federation
- /fsub (Fed ID): Subscribes your federation to the provided one
- /funsub (Fed ID): Unsubscribes your federation from the provided one
- /fsetlog (? Fed ID) (? chat/channel id) or /setfedlog (? Fed ID) (? chat/channel id): Sets a log chat or channel for your Federation
- /funsetlog (?Fed ID) or /unsetfedlog (?Fed ID): Unsets a federation log chat or channel
- /fexport (?Fed ID): Exports federation bans
- /fimport (?Fed ID) (file): Imports federation bans (Currently unsupported!)

**Only group owner**
- /fjoin (Fed ID) or /joinfed (Fed ID): Joins current chat into provided federation
- /fleave or /leavefed: Leaves current chat from the fed
- Avaible for Federation admins and owners
- /fchatlist (?Fed ID) or /fchats (?Fed ID): Shows a list of chats in the your federation list
- /fban (user) (?Fed ID) (?reason): Bans user in the federation (and all federations which subscribed to it)
- /sfban (user) (?Fed ID) (?reason): As above, but silently - means the messages about fbanning and the replied-to message (if was provided) will be removed
- /unfban (user) (?Fed ID) (?reason): Unbans a user from the federation
- /fadmins (?Fed ID): List all admins in this federation

**Avaible for all users**
- /fcheck (?user): Check user's federation ban info
- /finfo (?Fed ID): Shows info about the federation

**Examples**
*Basic things*
Let's create a new Federaion and connect it to a chat

- /fnew TestFederation
Creates a new Federation named TestFederation
Let's say that this Federation is having ID - `d6bfb2a3-9b16-4eb1-908f-bca56e613b8d`

`/fjoin d6bfb2a3-9b16-4eb1-908f-bca56e613b8d`
Joins the current chat to your Federation
⚠️ Only the chat owner is able to join its own chat to Federation

## Banning users
**Banning users across Federation, let's try to do it:**

- /fban @username
Bans the users with such username across all chats in the current Federation of the chat
You are able to use user ID instead of nickname, so the command will looks like `/fban 483808054`

- /fban
  
## Bans the replied user

- /fban @username Reason text
Bans the user with specific reason

- /fban `@username d6bfb2a3-9b16-4eb1-908f-bca56e613b8d`
Bans the user in the specific Federation

- /fban `@username d6bfb2a3-9b16-4eb1-908f-bca56e613b8d` Reason text
Bans the user in the specific Federation with specific reason

**In most cases you don't want to leave fban message and user's original message, so you are able to use /sfban @username, in this case Sophie will ban user and remove its process message, also if you are banning with replying, she will remove replied message also.**

Advanced Federaion administration
Let's check out advanced Federation administration things

- /fpromote will promotes a user to your Federation as its admin, such types of admins is allowed to ban/unban users in your Federation and see its info.
Well surely there is a way to reverse this action: just use /fdemote command

Logs. Do you want to store somewhere all banned users in your Federation and other its actions? Use Federation logs:
- /fsetlog `d6bfb2a3-9b16-4eb1-908f-bca56e613b8d` will sets a Federation log in current chat
- /fsetlog `d6bfb2a3-9b16-4eb1-908f-bca56e613b8d (chat_id):` Will sets a FedLog in specific chat, it's useful when you want to set a log channel (not chat)

Use /fexport to get a file with your Federation bans, you could add new ones and /fimport it, or copy Federation bans across many feds, use it as you want.

- /fchats command is able to show you a list of chats related to your Federation.

## Public Anti-spam Federations
**Federation ID: Name – Details**

`d6bfb2a3-9b16-4eb1-908f-bca56e613b8d: @OrangeFoxFed` – The Federation used for OrangeFox Recovery, bans all spammers across all OrangeFox chats and have many other trusted antispam feds connected.
`e5f6983a-3970-453e-80dd-5aaf7e154381: @OwlAntispam`
`845d33d3-0961-4e44-b4b5-4c57775fbdac: @DahuaEngine` – Powered by AI. Bans all spammers by prediction.
You'd like to add your own one?

Your Federation should follow some rules to be included here:

You have to only ban spammers.
The Federation should exist for Sophie only.
If you have succesfully followed those rules, you can PM @MrYacha (Telegram).
