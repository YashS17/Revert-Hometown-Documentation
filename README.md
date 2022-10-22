# About
Revert Hometown is a feature packed bot with auto moderation, logging, welcome and leave message, ticket, suggestions, nickname filter, account age, auto roles, voice roles, auto purge and more!
# Features
## Account Age
### Commands
  - **account-age**: Members joining the server with account age less than 7 days are banned automatically.
    - **Syntax**: `account-age <enable | threshold | show | disable>`
### Configuration
  - Customisable account age threshold (`account-age threshold days`).
## Auto Moderation
### Commands
  - **anti-profanity**: Removes the message of members when they post a blacklisted word.
    - **Syntax**: `automod anti-profanity <enable | punishment | punish-count | blacklist | whitelist | ignore | unignore | show | disable>`
  - **anti-link**: Removes the message of members when they post a link.
    - **Syntax**: `automod anti-link <enable | punishment | whitelist | blacklist | ignore | unignore | show | disable>`
  - **anti-caps**: Removes the message of members that have 70% of their characters capitalized.
    - **Syntax**: `automod anti-caps <enable| punishment | ignore | unignore | show | disable>`
  - **anti-spam**: Removes the message of members when they spam. Triggers when a member sends 5 messages during a 5 seconds timespan.
    - **Syntax**: `automod anti-spam <enable | punishment | ignore | unignore | show | disable>`
  - **attachment-spam**: Removes the message of members when they spam attachments.
    - **Syntax**: `automod attachment-spam <enable | punishment | punish-count | ignore | unignore | show | disable>`
  - **mention-spam**: Removes the message of members when they spam mentions.
    - **Syntax**: `automod mention-spam <enable | punishment | punish-count | ignore | unignore | show | disable>`
### Configurations
  - Ignore a channel/member/role for each auto moderation activity.
  - Set different punishments for each auto moderation activity.
  - Customisable mute duration.
  - Add a custom blacklisted word (`automod anti-profanity blacklist <word>`).
  - Add a custom whitelisted link (`automod anti-link whitelist <link>`).
## Auto Purge
### Command
  - **auto-purge**: New messages sent in a channel are deleted after certain duration.
    - **Syntax**: `auto-purge <enable | show | disable>`
### Configuration
  - Customisable duration after which the message will get deleted.
## Auto Responder
### Command
  - **auto-responder**: Trigger a auto responder
    - **Syntax**: `auto-responder <create | strict | startswith | endswith | toggle | list | edit | delete>`
### Configurations
  - Create any type of wildcard (`strict`, `startswith` and `endswith`).
  - Enable/disable a auto responder.
## Auto Roles
### Command
  - **auto-role**: A role which will be assigned to humans/bots on joining the server.
    - **Syntax**: `auto-role <add | delay | show | remove>`
### Configurations
  - Different roles for bots and humans.
  - Customisable delay after which the role will be assigned to the members.
## Command Enable/Disable
### Command
  - **command**: Enable/disable a command.
    - **Syntax**: `command <enable | show | disable>`
## Ignore Channel/Member
  - **ignore-channel**: Ignore a channel from using bot commands.
    - **Syntax**: `ignore-channel <add | show | remove>`
  - **ignore-member**: Ignore a member from using the bot.
    - **Syntax**: `ignore-member <add | show | remove>`
## Logging
### Commands
  - **message-delete**: Triggers the event when a message is deleted.
    - **Syntax**: `logging messagedelete [channel]`
  - **message-edit**: Triggers the event when a message is edited.
    - **Syntax**: `logging messageedit [channel]`
  - **member-update**: Triggers the event when a member's profile is updated. (Like: Discriminator, name, nickname, roles and avatar.)
    - **Syntax**: `logging memberupdate [channel]`
  - **member-bans**: Triggers the event when a member is banned/unbanned from the server.
    - **Syntax**: `logging memberbans [channel]`
  - **member-kick**: Triggers the event when a member is kicked from the server.
    - **Syntax**: `logging memberkick [channel]`
  - **server-update**: Triggers the event when the server is updated. (Like: Name, avatar, inactive channel, widget, etc.)
    - **Syntax**: `logging serverupdate [channel]`
  - **voice-update**: Triggers the event when a member is joining/moving/leaving between Voice channels.
    - **Syntax**: `logging voiceupdate [channel]`
  - **roles**: Triggers the event when a role is created/updated/deleted.
    - **Syntax**: `logging roles [channel]`
  - **channels**: Triggers the event when a channel is created/updated/deleted.
    - **Syntax**: `logging channels [channel]`
  - **threads**: Triggers the event when a thread is created/updated/deleted.
    - **Syntax**: `logging threads [channel]`
  - **join-leave**: Triggers the event when a member is joining/leaving the server.
    - **Syntax**: `logging joinleave [channel]`
  - **automod**: Triggers the event when an auto moderation avitvity takes place.
    - **Syntax**: `logging automod [channel]`
### Configurations
  - Ignore a channel/member/role for logging activities.
  - Specific channel for each event.
  - Detects new member's (to Discord) joining the server.
  - Disable all the logging events with one command (`logging disable-all`).
## Moderator Role
### Command
  - **mod-role**: Add a moderator role which will allow members to use all the moderation commands without having Manage Server permission.
    - **Syntax**: `mod-role <set | show | remove>`
## Muted Role
### Command
  - **muted-role**: Add a muted role which will be assigned to members when muted.
    - **Syntax**: `muted-role <set | create | show | remove>`
## Nickname Filter
### Command
  - **nickname-filter**: Members joining the server with blacklisted nicknames are automatically banned from the server.
    - **Syntax**: `nickname-filter <enable | blacklist | whitelist | show | disable>`
### Configuration
  - Add a blacklisted nickname (`nickname-filter blacklist <word>`).
## Suggestions
### Command
  - **suggestions**: Enable or disable suggestions in the server.
    - **Syntax**: `suggestions <set | approve | deny | delete | anonymous | show | disable>`
### Configuration
  - Approve or deny a member's suggestion.
  - Allow members to send suggestions anonymously.
## Ticket
### Commands
  - **ticket-config**: Ticket configuration of the server.
    - **Syntax**: `ticket-config <enable | message | panel | add-access | remove-access | rename | show | disable>`
  - **ticket**: Create, save, close or delete a ticket.
    - **Syntax**: `ticket <open | transcript | close | reopen | delete>`
### Configurations
  - Create a ticket panel (`ticket-config panel <create | show | delete>`).
  - Custom message which will be displayed in the ticket.
  - Add/remove access of a member from the ticket.
## Voice Roles
### Command
  - **voice-role**: A role which will be assigned to members on joining Voice Channels.
    - **Syntax**: `voice-role <add | show | remove>`
## Welcome and Leave
### Commands
  - **welcome**: Sends a message when a member joins the server.
    - **Syntax**: `welcome <enable | message | show | disable>`
  - **leave**: Sends a message when a member leaves the server.
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

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
