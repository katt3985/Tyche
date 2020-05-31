# Tyche
Tyche is a bot to roll dice, all results dictated by the Greek goddess of luck.

# Invite link
  use [this link](https://discordapp.com/oauth2/authorize?&client_id=631862376400158721&permissions=75776&scope=bot) to invite the bot to your server

# Command help
the default command prefix is `!` anyone can mention (@) the bot to get its current prefix
  
## !roll [!r]
 The roll command changes its behavior based on the game set for the channel.
 below are the differnt games currently reconized and some examples on how to use them

### Dungeons and Dragons 5th edition
  `!roll` : roll a d20 and return the result

  `!roll +1` : roll a d20, add 1, and return the result
  
  `!roll +5 for attack` : the "for attack" will be appended to the roll result
  
  `!roll -1 with disadvantage` : roll 2d20 and take the lower then subtract 1, other reconized words include: 'advantage', 'adv', and 'dis'
  
  `!roll 3d8` : include more than just a modifier and the phrase will be interpreted as a formula
  
### Chronicles of Darkness
  `!roll` : roll a 10 sided dice rerolling on a 10 and sum the number of dice that roll >= 8, standard check in Cof
  `!roll 3` : roll three 10 sided dice rerolling on a 10 and sum the number of dice that roll >= 8, standard check in CofD

  `!roll 5 with rote 9again` : roll 5 dice rerolling on a 9 or 10, and rerolling all failed results once
  
  `!roll 6 with 8again for perception` : roll 6 dice with '8again' (reroll on an 8, 9, or 10) and include "for perception" in the result
  
  `!roll 4 over 4 for researching in the library` : roll 4 dice 4 times for an extended check.

### Formula behavior (default behavior)
  this is always accessable via `!rollf` or `!rf`
  
  `!roll 1d6` : roll 1 die with 6 sides
  
  `!roll 4d6d1` : roll 4d6 but drop the lowest 1

  `!roll 4d6k3` : roll 4d6 but keep the top 3

  `!roll 5d10!` : roll 5d10, reroll dice that come up with 10 and include both in the result

  `!roll 5d10!8` : roll 5d10, same as above but reroll on an 8, 9, or 10
  
  `!roll 2d4*2` : roll 2 dice with 4 sides and multiply the result by 2
  
  `!roll (3 * 4) d (2 + 6)` : roll 12 dice with 8 sides
  
  `!roll 10*4*40+10*2` : do math
  
## !game [!games]
  `!game` : returns the current game for the channel, influences the `!roll` command
  
  `!game list` : list all the games that the bot knows and their codes, moderator only
  
  `!game set 0005` : sets the game for the channel to "Dungeons and Dragons 5th edition", moderator only

  `!game reset` : resets the channel to not have a game, `!roll` is now synonomous with `!rollf`
  
## !prefix (server moderator only)
  `!prefix /` : sets the bot's prefix to `/`
  
  `!prefix reset` : returns the bots prefit to `!`
