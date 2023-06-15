# **Minecraft Server - Java Edition - All Administrator Commands**

Here's the exhaustive list of all commands that can be used by the administrator of a Minecraft Server - Java Edition:

- Grant a player operator status:

    ```java
    op <player>
    ```

- Revoke a player's operator status:

    ```java
    deop <player>
    ```

- Ban a specific player:

    ```java
    ban <player>
    ```

- Unban a specific player:

    ```java
    unban <player>
    ```

- Ban a specific IP address:

    ```java
    ban-ip <address>
    ```

- Unban a specific IP address:

    ```java
    unban-ip <address>
    ```

- Add a player to the whitelist:

    ```java
    whitelist add <player>
    ```

- Remove a player from the whitelist:

    ```java
    whitelist remove <player>
    ```

- Turn the server whitelist on:

    ```java
    whitelist on
    ```

- Turn the server whitelist off:

    ```java
    whitelist off
    ```

- List all players on the whitelist:

    ```java
    whitelist list
    ```

- Kick a player from the server:

    ```java
    kick <player>
    ```

- Teleport one player to another:

    ```java
    tp <player1> <player2>
    ```

- Teleport a player to the specified coordinates:

    ```java
    tp <player> <x> <y> <z>
    ```

- Give a player a specific item and amount:

    ```java
    give <player> <item> [amount]
    ```

- Kill a player:

    ```java
    kill <player>
    ```

- Change the time of day:

    ```java
    time set <value>
    ```

- Change the weather:

    ```java
    weather clear/rain/thunder
    ```

- Change a player's game mode:

    ```java
    gamemode survival/creative/spectator/adventure <player>
    ```

- Give a player a specific amount of experience:

    ```java
    xp <amount> <player>
    ```

- Broadcast a message to all players:

    ```java
    say <message>
    ```

- Stop the server:

    ```java
    stop
    ```

- Force the server to write all pending changes to the disk:

    ```java
    save-all
    ```

- Disable automatic saving:

    ```java
    save-off
    ```

- Enable automatic saving:

    ```java
    save-on
    ```

- List all currently connected players:

    ```java
    list
    ```

- Reload the server configuration file:

    ```java
    reload
    ```

- Set the game difficulty:

    ```java
    difficulty peaceful/easy/normal/hard
    ```

- Clear all status effects from a player:

    ```java
    effect <player> clear
    ```

- Apply a status effect to a player for a given duration and potency:

    ```java
    effect <player> <effect> [seconds] [amplifier] [hideParticles]
    ```

- Display the world seed:

    ```java
    seed
    ```

- Set the world spawn:

    ```java
    setworldspawn [<x> <y> <z>]
    ```

- Set the default game mode:

    ```java
    defaultgamemode survival/creative/spectator/adventure
    ```

- Play a sound to a player:

    ```java
    playsound <sound> <player> <source> <x> <y> <z> <volume> <pitch>]<minimumVolume>
    ```

- Manage scoreboard objectives and players:

   ```java
   scoreboard objectives add <objective name> dummy <display-name>
   scoreboard objectives list

   ```