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

## Play a sound to a player

```java
playsound <sound> <player> <source> <x> <y> <z> <volume> <pitch> <minimumVolume>
```

In the context of the Minecraft `playsound` command, the `master` refers to the source channel of the sound being played.

Minecraft has various sound categories or "channels" that allow for more fine-tuned control over in-game audio settings. These categories can be individually adjusted by the player, meaning a player can make certain types of sounds louder or softer independent of other sounds.

Here are the main sound categories:

1. `master`: This is the main volume controller. All sounds in the game fall under this category.
2. `music`: This category is for the background music that plays while in the game.
3. `record`: This is for music disc sounds.
4. `weather`: This is for weather-related sounds (e.g., rain, thunder, etc.).
5. `block`: This is for sounds related to blocks (e.g., placing, breaking, stepping on blocks).
6. `hostile`: This is for sounds made by hostile creatures.
7. `neutral`: This is for sounds made by neutral creatures.
8. `player`: This is for sounds made by the player (e.g., damage, burp, etc.).
9. `ambient`: This is for ambient/environmental sounds.
10. `voice`: This is for any in-game voice output.

When you're using the `playsound` command and specify `master` as the source, the sound will play on the 'Master' channel, which means it is not categorized under any specific in-game sound like blocks, creatures, weather, etc. Instead, it plays as a general game sound that is controlled by the master volume setting in the game.

## Manage scoreboard objectives and players:

```java
scoreboard objectives add <objective name> dummy <display-name>
scoreboard objectives list
```
