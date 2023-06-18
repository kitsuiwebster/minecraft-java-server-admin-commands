# **Minecraft Server - Java Edition - All Administrator Commands (WIP)**

Here's the exhaustive list of all commands that can be used by the administrator of a Minecraft Server - Java Edition:

## Grant and revoke a player operator status:

```java
op <player>
deop <player>
```

### Player Parameter

`<player>` is the username of the player to whom you want to grant or revoke operator status.

## Ban and unban a specific player:

```java
ban <player>
pardon <player>
```

`<player>` is the username of the player that you want to ban or unban.

## Ban or unban a specific IP address:

```java
ban-ip <address>
pardon-ip <address>
```

`<address>` is the address of the player that you want to ban or unban.

## Add or remove a player to/from the whitelist:

```java
whitelist add <player>
whitelist remove <player>
```

`<player>` is the username of the player that you to add to/from the whitelist.

## Turn the server whitelist on/off:

```java
whitelist on
whitelist off
```

## List all players on the whitelist:

```java
whitelist list
```

## Kick a player from the server:

```java
kick <player>
```

## Teleport one player to another:

```java
tp <player1> <player2>
```

`<player1>` is the username of the player you want to teleport, and `<player2>` is the username of the player to whose location you want to teleport `<player1>`.

## Teleport a player to the specified coordinates:

```java
tp <player> <x> <y> <z>
```

`<player>` is the username of the player you want to teleport, and `<x> <y> <z>` are the coordinates to which you want to teleport the specified player.


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

### Syntax

- `<sound>` is the sound that will play (in your case, `minecraft:entity.creeper.primed`).
- `<source>` is the source of the sound (`master`, `music`, `record`, `weather`, `block`, `hostile`, `neutral`, `player`, `ambient`, `voice`).
- `<player>` is the player who will hear the sound (in your case, `KITSUI_WEBSTER`).
- `[<x> <y> <z>]` are the optional coordinates from where the sound will play (in your case, `-97 97 66`).
- `[<volume>]` is the optional volume, which controls how loud the sound will be (in your case, `10`).
- `[<pitch>]` is the optional pitch, which controls the tone of the sound (in your case, `1`).
- `[<minimumVolume>]` is the optional minimum volume for players who are outside the normal audible sphere.

### Source Parameter

In the context of the Minecraft `playsound` command, the `master` refers to the source channel of the sound being played.

Minecraft has various sound categories or "channels" that allow for more fine-tuned control over in-game audio settings. These categories can be individually adjusted by the player, meaning a player can make certain types of sounds louder or softer independent of other sounds.

Here are the main sound categories (sources):

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
