_Last updated 1/07/2022_

# Introduction

Anty is a multipurpose discord bot, here to make server management seamless, enhance your experience, and make complex tasks simple!

You can upvote Anty on the following sites:

- [Discordbotlist](https://discordbotlist.com/bots/anty/upvote)

**Useful Links**

- [Invite Link](https://discord.com/oauth2/authorize?client_id=896671807644532746&permissions=8&scope=guilds%20applications.commands%20bot%20email%20identify%20guilds.join)
- [Support Server](https://discord.gg/QgVU5q5ZvJ)
- [Anty's Website](https://anty.aspect.cx)
- [Dashboard](https://anty.aspect.cx/dashboard)
- [Anty API](https://anty.aspect.cx/api/stats)
- [Reddit](https://www.reddit.com/r/AntyBot/)
- [GitHub Organisation](https://github.com/AntyBot)

# Documentation

**Who the documentation is for**
This documentation is designed for moderators. If you are just looking for the list of commands, you can find them [here](https://anty.aspect.cx/commands) or by using the `help` command.

**Preface Notes**
Commands shown in this documentation will be represented without a prefix. For example, instead of `=help` or `/help`, the documentation will just show `help`. This is because both prefix and slash commands are supported, with prefix commands changable per server.

`[]` is used for required command options. For example `ban [user]`, where the user option is required for the command to work. `()` is used for optional command options. For example `ban [user] (reason)`, where reason is an optional input, meaning the command will work without providing a reason.

You will find a table of commands for each category within a module, or someone one per module. Above the table, the default setting for who can use the commands will be specified.

| Table of Contents                |
| -------------------------------- |
| [1. Moderation](#1-moderation)   |
| [2. Information](#2-information) |

## 1. Moderation

### 1.1 Users

By default, these commands can only be used by users with the `ADMINISTRATOR` permission or users with the assigned moderator role.

| Command      | Description               | Usage                                |
| ------------ | ------------------------- | ------------------------------------ |
| `ban`        | Ban a user                | `ban [user] (reason)`                |
| `kick`       | Kick a user               | `kick [user]`                        |
| `nick`       | Change your nickname      | `nick [nickname]`                    |
| `removewarn` | Remove a warn using an ID | `removewarn [id]`                    |
| `timeout`    | Timeout a user            | `timeout [user] (duration) (reason)` |
| `unban`      | Unban a user              | `unban [user]`                       |
| `warn`       | Warn a user               | `warn [user] [reason]`               |
| `warnings`   | Returns a users warnings  | `warnings (user)`                    |
| `mute`       | Mute a user               | `mute [user] (duration) (reason)`    |
| `unmute`     | Unmute a user             | `unmute [user]                       |

### 1.2 Channels

By default, these commands can only be used by users with the `ADMINISTRATOR` permission or users with the assigned moderator role.

| Command  | Description                                                   | Usage                   |
| -------- | ------------------------------------------------------------- | ----------------------- | ------------------ |
| `clear`  | Deletes a specified number of messages from a channel or user | `clear [amount] (user)` |
| `lock`   | Lock a channel                                                | `lock (channel)`        |
| `unlock` |                                                               | Unlock a channel        | `unlock (channel)` |

### 1.3 Logging

By default, these commands can only be used by users with the `ADMINISTRATOR` permission or users with the assigned moderator role.

**Commands**

| Command     | Description                         | Usage                   |
| ----------- | ----------------------------------- | ----------------------- |
| log channel | Set the log channel                 | `log channel [channel]` |
| log disable | Disable loggin                      | log disable             |
| log enable  | enable logs if previously disabled. | log enable              |

Anty will log specified events to your selecting logging channel. Logs are sent via webhooks.

**Events**

| Client                        |
| ----------------------------- |
| Log channel set               |
| Log channel set               |
| Suspicious behaviour detected |
| Blacklisted words             |
| Moderator command used        |

| Messages              |
| --------------------- |
| Message deleted       |
| Message edited        |
| Bulk deleted messages |

| Member                   |
| ------------------------ |
| Member joined            |
| Member left              |
| Member added to role     |
| Member removed from role |
| Nickname updated         |
| Member banned            |
| Member unbanned          |

| Server                                    |
| ----------------------------------------- |
| Server name changed                       |
| Server icon changed                       |
| Server shard changed                      |
| Server splash changed                     |
| Server banned changed                     |
| Server description changed                |
| Server verification changed               |
| Server vanity URL changed                 |
| Server NSFW level changed                 |
| Server Discovery Splash Changed           |
| Server Progress Bar Changed               |
| Server AFK Timeout Changed                |
| Server AFK Channel Changed                |
| Server System Channel Changed             |
| Server Premium Tier Changed               |
| Server Premium Subscription Count Changed |
| Server Content Filter Changed             |
| Server MFA Level Changed                  |
| Server Notifications Changed              |
| Server Rules Channel Changed              |
| Server Moderator Channel Changed          |
| Server Primary Language Changed           |
| Server Owner Changed                      |
| Server Featured Updated                   |

| Role Events  |
| ------------ |
| Role Created |
| Role Deleted |

| Channel Events                      |
| ----------------------------------- |
| Channel Created                     |
| Channel Deleted                     |
| Channel Message Pins Updated        |
| Channel Name Updated                |
| Channel Topic Updated               |
| Channel Type Updated                |
| Channel NSFW Updated                |
| Channel Rate Limit Per User Updated |

| Voice Events                       |
| ---------------------------------- |
| Voice Channel Joined (Coming Soon) |
| Voice Channel Left (Coming Soon)   |
| Voice Channel Moved (Coming Soon)  |

## 2. Information

### 2.1 Client

By default, these commands can be used by `@everyone`.

| Command         | Description                                                        | Usage                            |
| --------------- | ------------------------------------------------------------------ | -------------------------------- |
| `help`          | Show information about the bot and all commands                    | `help`                           |
| `info`          | Shows information about the bot                                    | `info`                           |
| `ping`          | Returns Anty's latency                                             | `ping`                           |
| `search server` | Search for server(s) that correlate to the chosen method and input | `search server [method] [input]` |
| `stats`         | Returns Anty's stats                                               | `stats`                          |
| `troubleshoot`  | Get information on how to resolve common issues                    | `troubleshoot`                   |
| `uptime`        | Returns how long Anty has been online since last reboot            | `uptime`                         |
|                 |                                                                    |                                  |

### 2.2 Server

By default, these commands can be used by `@everyone`.

| Command               | Description                                      | Usage                 |
| --------------------- | ------------------------------------------------ | --------------------- |
| `invites`             | Returns invite links for the server              | `invites`             |
| `serverinfo`          | Returns information about the server             | `serverinfo`          |
| `serverinfo general`  | Returns information about the server             | `serverinfo general`  |
| `serverinfo users`    | Returns users stats for the server               | `serverinfo users`    |
| `serverinfo channels` | Returns channel stats for the server             | `serverinfo channels` |
| `serverinfo stats`    | Returns general stats for the server             | `serverinfo stats`    |
| `serverinfo owner`    | Returns user information of the servers owner    | `serverinfo owner`    |
| `prefix`              | Return the current prefix for Anty on the server | `prefix`              |

### 2.3 User

By default, these commands can be used by `@everyone`.

| Command  | Description                 | Usage           |
| -------- | --------------------------- | --------------- |
| `avatar` | Returns Diep.io party links | `avatar (user)` |

### 2.4 Games

By default, these commands can be used by `@everyone`.

| Command | Description                 | Usage           |
| ------- | --------------------------- | --------------- |
| `diep`  | Returns Diep.io party links | `diep (reigon)` |

### 2.5 Other

By default, these commands can be used by `@everyone`.

| Command  | Description                    | Usage             |
| -------- | ------------------------------ | ----------------- |
| `domain` | Check if a domain is available | `domain [domain]` |

## Profile

By default, these commands can be used by `@everyone` and have a global effect.

| Command        | Description | Usage |
| -------------- | ----------- | ----- |
| `profile`      |             |       |
| `bio`          |             |       |
| `achievements` |             |       |
|                |             |       |
|                |             |       |
|                |             |       |
|                |             |       |
|                |             |       |
|                |             |       |
|                |             |       |

## Music

By default, these commands can be used by `@everyone`.

| Command      | Description                                            | Usage                 |
| ------------ | ------------------------------------------------------ | --------------------- |
| `lyrics`     | Display lyrics for the current song or a specific song | `lyrics [song]`       |
| `nowplaying` | Shows information about the current song               | `nowplaying`          |
| `pause`      | Pause the current song `pause`                         | `pause`               |
| `play`       | Play a song                                            | `play [song]`         |
| `queue`      | Display the song queue                                 | `queue`               |
| `resume`     | Resume the current song                                | `resume`              |
| `skip`       | Skip the current song                                  | `skip`                |
| `volume`     | Change or check the volume of the current song         | `volume [percentage]` |

## System

### Server Configuration

By default, these commands can only be used by users with the `ADMINISTRATOR` permission or with the assigned moderator role.

| Command              | Description                                            | Usage                |
| -------------------- | ------------------------------------------------------ | -------------------- | ------- | ------------------------------------------------------------ |
| `autonick`           | Automatically nickname users when they join the server | `autonick [format]`  |
| `buttonroles`        | Configure buttons on a role message                    | `buttonroles`        |
| `dropdownroles`      | Configure dropdowns on a role message                  | `dropdownroles`      |
| `filter`             | Simple chat filtering system                           | `filter`             |
| `giveaway`           | Giveaway system                                        | `giveaway`           |
| `rolemessage`        | Add a role message                                     | `rolemessage`        | `roles` | Manage roles, with related messages, buttons, and dropdowns. |
| `rolesetup`          | Setup roles (Use in the roles channel!)                | `rolesetup`          |
| `setprefix`          | Set the prefix for the server                          | `setprefix`          |
| `settings`           | Manage settings for the server                         | `settings`           |
| `ticketsetup`        | Setup a new ticketing system                           | `ticketsetup`        |
| `verify`             | Verify yourself in for a server                        | `verify`             |
| `verification setup` | Setup verification for a server                        | `verification setup` |

### User Settings

By default, these commands can be used by `@everyone`, and are per-guild commands. This means that these commands only have an effect in the server they are executed in.

| Command  | Description                     | Usage           |
| -------- | ------------------------------- | --------------- |
| `afk`    | Set AFK status                  | `afk (message)` |
| `ticket` | Ticket action                   | `ticket`        |
| `Voice`  | Manage your VC's voice settings |                 |

## Miscellaneous

### Server

By default, these commands can be used by `@everyone`.

| Command   | Description                                | Usage     |
| --------- | ------------------------------------------ | --------- |
| `poll`    | Create a poll                              | `poll`    |
| `suggest` | Create a suggestion in an organized matter | `suggest` |

### Tools

By default, these commands can be used by `@everyone`.

| Command      | Description                       | Usage        |
| ------------ | --------------------------------- | ------------ |
| `echo`       | Echos your input                  | `echo`       |
| `lorem`      | Returns dummy text                | `lorem`      |
| `calculator` | Use the advanced calculator       | `calculator` |
| `website`    | Returns important website links   | `website`    |
| `msgdevs`    | Send a message to Anty Developers | `msgdevs`    |

## Fun & Entertainment

By default, these commands can be used by `@everyone`.

| Command   | Description                                                   | Usage     |
| --------- | ------------------------------------------------------------- | --------- |
| `love`    | Calculate the love affinity you have for another person.      | `love`    |
| `meme`    | Sends an epic meme.                                           | `meme`    |
| `handrps` | Same as Rock Paper Scissors, but with hand emojis.            | `handrps` |
| `rps`     | Rock Paper Scissors game. React to one of the emojis to play. | `rps`     |

## Additional Notes

### Status

Anty's status is updated every minute. So, when Anty is added to a new server, you will see the number increase within the next minute!

### Super Commands

Super commands are original commands Anty provides which other discord bots typically don't support. These commands are available to Beta Testers, Premium Users, Anty Developers, and Aspect's Discord Staff.
