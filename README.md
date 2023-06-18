# **Minecraft Server - Java Edition - All Administrator Commands (WIP)**

Here's the exhaustive list of all commands that can be used by the administrator of a Minecraft Server - Java Edition:

## Grant and revoke a player operator status

```java
op <player>
deop <player>
```

### Player Parameter

`<player>` is the username of the player to whom you want to grant or revoke operator status.

## Ban or unban a specific player

```java
ban <player>
pardon <player>
```

`<player>` is the username of the player you want to ban or unban.

## Ban or unban a specific IP address

```java
ban-ip <address>
pardon-ip <address>
```

`<address>` is the address of the player you want to ban or unban.

## Add or remove a player to/from the whitelist

```java
whitelist add <player>
whitelist remove <player>
```

`<player>` is the username of the player you want to add to/from the whitelist.

## Turn the server whitelist on/off

```java
whitelist on
whitelist off
```

## List all players on the whitelist

```java
whitelist list
```

## Kick a player from the server

```java
kick <player>
```

`<player>` is the username of the player you want to kick from the server.

## Teleport one player to another

```java
tp <player1> <player2>
```

`<player1>` is the username of the player you want to teleport, and `<player2>` is the username of the player to whose location you want to teleport `<player1>`.

## Teleport a player to the specified coordinates

```java
tp <player> <x> <y> <z>
```

`<player>` is the username of the player you want to teleport, and `<x> <y> <z>` are the coordinates to which you want to teleport the specified player.

## Give a player a specific item and amount

```java
give <player> <item> [amount]
```

`<player>` is the username of the player to whom you want to give an item, `<item>` is the specific item you want to give, and `[amount]` is an optional parameter that defines the quantity of the item to be given.

### Item Parameter

To give an item, you use its item ID in the give command. The item ID is usually in the format minecraft:item_name. For example, to give an oak log, you would use minecraft:oak_log. You can find all item IDs [Here](https://minecraftitemids.com/).

## Kill a player

```java
kill <player>
```

`<player>` is the username of the player you want to immediately eliminate from the game, causing them to respawn.

## Change the time of day

```java
time set <value>
```

## Change the weather

```java
weather <weather>

```

### Weather Parameter

1. `clear`: To set the sun.
2. `rain`: To set the rain.
3. `thunder`: To set the rain and the thunder.

## Change a player's game mode

```java
gamemode <gamemode> <player>
```

### Game Mode Parameter

1. `survival`: To set the game mode to survival.
2. `creative`: To set the game mode to creative.
3. `spectator`: To set the game mode to spectator.
4. `adventure`: To set the game mode to adventure.

## Give a player a specific amount of experience

```java
xp add <player> <amount> points
xp add <player> <amount> levels
```

`<player>` is the username of the player to whom you want to give experience points, and `<amount>` is the number of experience points or levels to be given.

## Broadcast a message to all players

```java
say <message>
```

`<message>` represents the content of the message that you want to broadcast to all players on the server.

## Stop the server

```java
stop
```

## Reload the server configuration file

```java
reload
```

## Force the server to write all pending changes to the disk

```java
save-all
```

## Disable and enable automatic saving

```java
save-off
save-on
```

## List all currently connected players

```java
list
```

## Set the game difficulty

```java
difficulty <difficulty>
```

### Difficulty Parameter

1. `peaceful`: To set the difficulty to peaceful.
2. `easy`: To set the difficulty to easy.
3. `normal`: To set the difficulty to normal.
4. `hard`: To set the difficulty to hard.

## Clear all status effects from a player

```java
effect <player> clear
```

`<player>` is the username of the player from whom you want to remove all active status effects.

## Apply a status effect to a player for a given duration and potency

```java
effect <player> <effect> [seconds] [amplifier] [hideParticles]
```

- `<player>` is the username of the player to whom you want to apply a status effect
- `<effect>` is the ID of the status effect. You can find all effect IDs [here](https://www.digminecraft.com/lists/effect_list_pc.php).
- `[seconds]` is the optional duration of the effect in seconds.
- `[amplifier]` is the optional level of the effect (starting from 0).
- `[hideParticles]` is an optional boolean value (true or false) that, if set to true, hides particles from the effect.

## Display the world seed

```java
seed
```

## Set the world spawn

```java
setworldspawn [<x> <y> <z>]
```

- `[<x> <y> <z>]` are parameters that represent the coordinates where you want to set the world spawn point.

## Set the default game mode

```java
defaultgamemode <defaultgamemode>
```

### Default Game Mode Parameter

1. `survival`: To set the default game mode to survival.
2. `creative`: To set the default game mode to creative.
3. `spectator`: To set the default game mode to spectator.
4. `adventure`: To set the default game mode to adventure.

## Play a sound to a player

```java
playsound <sound> <player> <source> [<x> <y> <z>] <volume> <pitch> <minimumVolume>
```

### Parameters

- `<sound>` is the sound that will play (in your case, `minecraft:entity.creeper.primed`).
- `<source>` is the source of the sound (`master`, `music`, `record`, `weather`, `block`, `hostile`, `neutral`, `player`, `ambient`, `voice`).
- `<player>` is the player who will hear the sound.
- `[<x> <y> <z>]` are the coordinates from where the sound will play.
- `[<volume>]` is the volume, which controls how loud the sound will be.
- `[<pitch>]` is the pitch, which controls the tone of the sound.
- `[<minimumVolume>]` is the minimum volume for players who are outside the normal audible sphere.

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

## Manage scoreboard objectives and players

```java
scoreboard objectives add <objective name> dummy <display-name>
scoreboard objectives list
```
