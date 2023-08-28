## Privacy with Sophie

:information_source: Sophie respects your privacy; every part of Sophie is open source!
- `Sophie's team is constantly improving privacy and security.`

  
* We don't collect your private data!
- `We don't save your messages or any other information about them.`

## What data we are saving

 **Public user's data**

First and second names,
User ID, Telegram username
Telegram language
Timestamp of the date when Sophie had seen the user first time

**Chat data**

Chat name,
username, and Chat ID
We are caching chat admins (1 hour after the last command)

We are not logging message counts, messages texts, or their authors!

**Analytics**

Speed of long queries
Counting of data types in all chats
Percents of using features in chats
Number of new chats in 48 hours

# Crashlytics
Crashlytics significantly help Sophie to be stable. We are trying to log as few data as possible.

**Currently we can only log:**

Crash traceback
Raw update data which caused crash (with censored private information)


**Raw update example:**

```python
{
   "message_id":[
      "HIDDEN"
   ],
   "from":[
      "HIDDEN"
   ],
   "chat":[
      "HIDDEN"
   ],
   "date":1588430258,
   "text":"\/adminlist",
   "entities":[
      {
         "offset":0,
         "length":10,
         "type":"bot_command"
      }
   ],
   "reply_to_message":[
      "HIDDEN"
   ]
}
