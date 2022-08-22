# Auto Moderation
## Commands
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
## Configurations
  - Ignore a channel/member/role for each auto moderation activity.
  - Set different punishments for each auto moderation activity.
  - Customisable mute duration.
  - Add a custom blacklisted word.
  - Add a custom whitelisted link.
# Logging
## Commands
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
## Configurations
  - Ignore a channel/member/role for logging activities.
  - Specific channel for each event.
  - Detects new member's (to Discord) joining the server.
  - Disable all the logging events with one command (`logging disable-all`).
