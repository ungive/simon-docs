# **Simon**
[![YGOPro Percy](http://i.imgur.com/v732Scx.png)](https://discord.gg/Rae2vZV)

*All commands are case-insensitive.*  
### Commands
* [`Card Search`](#card-search)
* [`Pack Opening`](#pack-opening)
* [`Trivia Game`](#trivia-game)
* [`Scripting Library`](#scripting-library)
  * [`Constants`](#constants)
  * [`Functions`](#functions)
  * [`Parameters`](#parameters)
  * [`Page Browsing`](#page-browsing)
  * [`Descriptions`](#descriptions)
* [`About`](#about)


---

### **Card Search**

>**Type `<card_name[, input_language][, output_language]>` to search for a Yu-Gi-Oh! card.**  
Searching with `{}` instead of `<>` results in a more compact response.

*`<Kuriboh>` gives the following result:*  
![Card Search - Kuriboh](http://image.prntscr.com/image/72822c5ccc7c452e939ca83d5627f431.png)

>The following languages are available (Default: `en`):  
English (`en`), German (`de`), French (`fr`), Italian (`it`), Spanish (`es`), Japanese (`ja`), Chinese (`ch`) and Taiwanese (tw).  

*`<Bunilla, en, ja>` accesses the japanese database by only giving the english card name:*  
![Card Search - Bunilla](http://image.prntscr.com/image/43b3519b8db24684a14c25092d74bf4d.png)

---

### **Pack Opening**

>**Type `.packopen [format] [language] [pack_name]` to open a pack.**  
**Format**: `TCG` or `OCG` (Default: `TCG`)  
**Language**: `en`, `de`, `fr`, `it`, `es`, `ja` or `cn` (Default: `en`).  
**Pack name**: The name of any Yu-Gi-Oh! pack.
**Alias**: `.po`  

*`.po Breakers of Shadow` opens a pack with nine random cards, containing one holo, one rare and seven common cards:*  
![Pack Opening - Breakers of Shadow](http://image.prntscr.com/image/8d66b367c27d46b29e184cfcac39077b.png)

---

### **Trivia Game**

>**Type `.trivia [format] [end_score]` to play the trivia game.**  
The goal of the game is to guess the name of a card as fast as possible by only looking at its picture.  
**Format**: `Anime`, `TCG`, `OCG` (Default: all)  
**End score**: The number of points that are needed to win the game. A scoreboard is displayed after each card (Default: 1).   
**Alias**: `.t`  

>**Type `.trivaquit` to stop the game.**  
Only the creator of the game and certain roles or users whitelisted in the server config are permitted to do this.  
**Alias**. `.tq`  

*`.t 10` starts a game that ends when someone reaches 10 points:*  
![Trivia Game - Z-ONE](http://image.prntscr.com/image/9f22ade0b6f14bbe8757440d52f60419.png)

--

### Server List

>**Type `.servers` to get a list of servers Simon is operating on.**  


---

### Scripting Library

**Note:** This series of commands is dedicated to the scripters of the YGOPro game and those that want to be part of those.  
If you are interested in scripting Yu-Gi-Oh! cards join the `scripting_lua_101` channel on the YGOPro Percy server.  
An Invitation link can be found at the top of this file.  

--

#### Constants

>**Type `.constant [keyword]` to search for a YGOPro Lua constant.**  
**Keyword**: The word that the your constant contains.  
**Alias**: `.c`  
The result is formatted like this: `[index] hex_code | constant_name`.  

*`.constant effect`:*  
![Scripting Library - Constant](http://image.prntscr.com/image/70427f3c334b49bb972258397f41c4fd.png)

--

#### Functions

>**Type `.function [keyword]` to search for a YGOPro Lua function.**  
**Keyword**: The word that the your function contains.  
**Alias**: `.f`  
The result is formatted like this: `[index] return_type | function_name(params)`.  

*`.function draw`:*  
![Scripting Library - Function](http://image.prntscr.com/image/357524c4c9c547babd3d8178b752410c.png)

--

#### Parameters

>**Type `.parameter [keyword]` to search for a parameter of a YGOPro Lua function.**  
**Keyword**: The word that the the parameter of a function contains.  
**Alias**: `.param`  
The result is formatted like this: `[index] type | parameter_name`.  

*`.param player`:*  
![Scripting Library - Parameter](http://image.prntscr.com/image/b7dd0266a98d4f0cac5212ad0b4eff82.png)

--

#### Page Browsing

>**Type `.page [page_number]` to browse a page.**  
Displays the content of the next page by editing the last search response message.  
**Page number**: The page you want to be displayed.  
The current page number is displayed at the bottom of the response message of your search.  
You can also edit the page number of your previous `.page` message for more comfort.  
**Alias**: `.p`  

*`.page 2`:*  
![Scripting Library - Page](http://image.prntscr.com/image/94a4994324b14dbda9a0a7fa0a8773b8.png)

--

#### Descriptions

>**Type `.description [index]` to show the description of a result at an index.**  
Displays the descriptiong of a result at an index by editing the last search response message.  
**Index**: The index.  
The index of a result is displayed at the very left of its line.  
You can also edit the index of your previous `.description` message for more comfort.  
**Aliases**: `.desc` and `.d`  

*`.description 2`:*  
![Scripting Library - Page](http://image.prntscr.com/image/fffd5cbb7a744390b15977916448fd4c.png)

---

### About

Simon is written with Discord<span></span>.NET in C# by Jonas Vanen aka Snrk.
You can talk to me on Discord (Snrk#9259).

