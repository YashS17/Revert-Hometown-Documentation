# About
Revert Hometown is a feature packed bot with auto moderation, logging, welcome and leave message, ticket, suggestions, nickname filter, account age, auto roles, voice roles, auto purge and more!
# Features
## Auto Moderation
### Commands
  - **Anti Profanity**: Removes the message of members when they post a blacklisted word.
    - **Syntax**: `automod anti-profanity <enable | punishment | punish-count | blacklist | whitelist | ignore | unignore | show | disable>`
  - **Anti Link**: Removes the message of members when they post a link.
    - **Syntax**: `automod anti-link <enable | punishment | whitelist | blacklist | ignore | unignore | show | disable>`
  - **Anti Caps**: Removes the message of members that have 70% of their characters capitalized.
    - **Syntax**: `automod anti-caps <enable| punishment | ignore | unignore | show | disable>`
  - **Anti Spam**: Removes the message of members when they spam. Triggers when a member sends 5 messages during a 5 seconds timespan.
    - **Syntax**: `automod anti-spam <enable | punishment | ignore | unignore | show | disable>`
  - **Attachment Spam**: Removes the message of members when they spam attachments.
    - **Syntax**: `automod attachment-spam <enable | punishment | punish-count | ignore | unignore | show | disable>`
  - **Mention Spam**: Removes the message of members when they spam mentions.
    - **Syntax**: `automod mention-spam <enable | punishment | punish-count | ignore | unignore | show | disable>`
### Configurations
  - Ignore a channel/member/role for each auto moderation activity.
  - Set different punishments for each auto moderation activity.
  - Customisable mute duration.
  - Add a custom blacklisted word (`automod anti-profanity blacklist <word>`).
  - Add a custom whitelisted link (`automod anti-link whitelist <link>`).
## Logging
### Commands
  - **Message Delete**: Triggers the event when a message is deleted.
    - **Syntax**: `logging messagedelete [channel]`
  - **Message Edit**: Triggers the event when a message is edited.
    - **Syntax**: `logging messageedit [channel]`
  - **Member Update**: Triggers the event when a member's profile is updated. (Like: Discriminator, name, nickname, roles and avatar.)
    - **Syntax**: `logging memberupdate [channel]`
  - **Member Bans**: Triggers the event when a member is banned/unbanned from the server.
    - **Syntax**: `logging memberbans [channel]`
  - **Member Kick**: Triggers the event when a member is kicked from the server.
    - **Syntax**: `logging memberkick [channel]`
  - **Server Update**: Triggers the event when the server is updated. (Like: Name, avatar, inactive channel, widget, etc.)
    - **Syntax**: `logging serverupdate [channel]`
  - **Voice Update**: Triggers the event when a member is joining/moving/leaving between Voice channels.
    - **Syntax**: `logging voiceupdate [channel]`
  - **Roles**: Triggers the event when a role is created/updated/deleted.
    - **Syntax**: `logging roles [channel]`
  - **Channels**: Triggers the event when a channel is created/updated/deleted.
    - **Syntax**: `logging channels [channel]`
  - **Threads**: Triggers the event when a thread is created/updated/deleted.
    - **Syntax**: `logging threads [channel]`
  - **Join/Leave**: Triggers the event when a member is joining/leaving the server.
    - **Syntax**: `logging joinleave [channel]`
  - **Automod**: Triggers the event when an auto moderation avitvity takes place.
    - **Syntax**: `logging automod [channel]`
### Configurations
  - Ignore a channel/member/role for logging activities.
  - Specific channel for each event.
  - Detects new member's (to Discord) joining the server.
  - Disable all the logging events with one command (`logging disable-all`).
## Welcome and Leave
### Commands
  - **Welcome**: Sends a message when a member joins the server.
    - **Syntax**: `welcome <enable | message | show | disable>`
  - **Leave**: Sends a message when a member leaves the server.
    - **Syntax**: `leave <enable | message | show | disable>`
### Variables
  - `(user.display_name)`: Member's name without discriminator. For example, `TSRxZeusOP`.
  - `(user.name)`: Member's name with discriminator. For example, `TSRxZeusOP#3470`.
  - `(user.mention)`: Mentions the member. For example, `@TSRxZeusOP`.
  - `(user.created_at)`: Member's account creation date.
  - `(server.name)`: Server's name.
  - `(server.member_count)`: Server's member count.
### Configuration
  - Set a custom message.
## Ticket
### Commands
  - **Ticket Config**: Ticket configuration of the server.
    - **Syntax**: `ticket-config <enable | show | panel | add-access | remove-access | rename | disable>`
  - **Ticket**: Create, save, close or delete a ticket.
    - **Syntax**: `ticket <open | transcript | close | delete>`
### Configurations
  - Create a ticket panel (`ticket-config panel <create | show | delete>`).
  - Custom message which will be displayed in the ticket.
  - Add/remove access of a member from the ticket.
## Suggestions
### Commands
  - **Suggestions**: Enable or disable suggestions in the server.
    - **Syntax**: `suggestions <set | approve | deny | anonymous | show | disable>`
### Configuration
  - Approve or deny a member's suggestion.
  - Allow members to send suggestions anonymously.
## Nickname Filter
### Commands
  - **Nickname Filter**: Members joining the server with blacklisted nicknames are automatically banned from the server.
    - **Syntax**: `nickname-filter <enable | blacklist | whitelist | show | disable>`
### Configuration
  - Add a blacklisted nickname (`nickname-filter blacklist <word>`).
## Account Age
### Commands
  - **Account Age**: Members joining the server with account age less than 7 days are banned automatically.
    - **Syntax**: `account-age <enable | threshold | show | disable>`
### Configuration
  - Customisable account age threshold.
## Auto Roles
### Commands
  - **Auto Role**: A role which will be assigned to humans/bots on joining the server.
    - **Syntax**: `auto-role <add | delay | show | remove>`
### Configurations
  - Different roles for bots and humans.
  - Customisable delay after which the role will be assigned to the members.
## Voice Roles
### Commands
  - **Voice Role**: A role which will be assigned to members on joining Voice Channels.
    - **Syntax**: `voice-role <add | show | remove>`
## Auto Purge
### Commands
  - **Auto Purge**: New messages sent in a channel are deleted after certain duration.
    - **Syntax**: `auto-purge <enable | show | disable>`
### Configuration
  - Customisable duration after which the message will get deleted.
