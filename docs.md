
# Quick links

- Main things
  - [functions](#functions)
  - [structures](#structures)
  - [enums](#enums)
<!-- - Example scripts
  - [world clear]() 
- Tutorials
  - [convert Pandora functions to GrowBot]() -->


---

# Functions

This section provides detailed documentation for GrowBot functions. Below, you will find tables showcasing all the functions available in the GrowBot Lua API, accompanied by concise descriptions of their functionality. To explore a specific function further, simply click on its name, represented like [this](#this). This will provide you with comprehensive information including its syntax, parameters, return values, additional remarks, and practical usage examples.

- Quick links
  - [connection functions](#connection-functions)
  - [bot functions](#bot-functions)
  - [packet functions](#packet-functions)
  - [proxy functions](#proxy-functions)
  - [callback functions](#callback-functions)
  - [world functions](#world-functions)
  - [inventory functions](#inventory-functions)
  - [player functions](#player-functions)
  - [tile functions](#tile-functions)
  - [text_packet functions](#text_packet-functions)
  - [variant functions](#variant-functions)
  - [bot_manager functions](#bot_manager-functions)
  - [item_manager functions](#item_manager-functions)
  - [other functions](#other-functions)

---

## connection functions
| Function | Description |
|  :----: |  ---- |
| [connect](#connect) | Connects bot to growtopia server. |
| [disconnect](#disconnect) | Diconnects bot from growtopia server. |
| [reconnect](#reconnect) | Reconnects bot. |

## bot functions
| Function | Description |
|  :----: | ---- |
| [set_pos](#set_pos) | Sets bot to the specified position. |
| [set_pos_at_tile](#set_pos_at_tile) | Sets bot to the specified tile position. |
| [place_tile](#place_tile) | Bot places specified tile to the specified tile position. |
| [punch_tile](#punch_tile) | Bot punches the specified tile position. |
| [wrench_tile](#wrench_tile) | Bot wrenches the speficied tile position. |
| [activate_tile](#activate_tile) | Bot activates the specified tile positon. |
| [activate_item](#activate_item) | Bot activates the specified item. |
| [collect_item](#collect_item) | Collects item. |
| [collect_items](#collect_items) | Collects all items around. |
| [set_bubble](#set_bubble) | Sets the bubble like `brb`, |
| [say](#say) | Says a message to chat. |
| [warp](#warp) | Goes to the specified world. |
| [exit_world](#exit_world) | Exits the world. |
| [set_mac](#set_mac) | Sets specified mac for bot. |
| [set_action](#set_action) | Sets specified action text for bot. |
| [find_path](#find_path) | Finds path in world to the specified destination. |
| [get_local_player](#get_local_player) | Gets the bot's player structure. |
| [get_inventory](#get_inventory) | Gets the bot's player inventory structure. |

## packet functions
| Function | Description |
|  :----: | ---- |
| [send_generic_text](#send_generic_text) | Sends specified generic packet. |
| [send_game_message](#send_game_message) | Sends specified game message packet. |
| [send_game_packet](#send_game_packet) | Sends specified game packet. |

## proxy functions
| Function | Description |
|  :----: | ---- |
| [set_proxy](#set_proxy) | Sets the bot proxy. |
| [set_proxy_auth](#set_proxy_auth) | Sets bot proxy authentication. |
| [get_ping](#get_ping) | Gets bot current bot ping. |
| [get_proxy_reply](#get_proxy_reply) | Gets last proxy reply. |
| [get_proxy_string](#get_proxy_string) |  Get proxy in a string format like ip:port:user:pass. |

## callback functions
| Function | Description |
|  :----: | ---- |
| [remove_callback](#remove_callback) | Removes specific callback. |
| [has_callback](#has_callback) | Checks is specified callback exists. |
| [add_game_message_callback](#add_game_message_callback) | Adds specified game message callback. |
| [add_game_packet_callback](#add_game_packet_callback) | Adds specified game packet callback. |
| [add_function_call_callback](#add_function_call_callback) | Adds specified function call callback. |
| [add_track_packet_callback](#add_track_packet_callback) | Adds specified track packet callback. |

## world functions
| Function | Description |
|  :----: | ---- |
| [get_world](#get_world) | Gets the world structure. |
| [get_tile](#get_tile) | Gets the tile specified by position. |
| [get_tiles](#get_tiles) | Get a table of all world tiles. |
| [get_world_object](#get_world_object) | Gets specific world object. |
| [get_world_objects](#get_world_objects) | Gets a table of all world objects. |
| [get_player](#get_player) | Gets specific player in world. |
| [get_players](#get_players) | Gets a table of all world players. |
| [get_npc](#get_npc) | Gets specific npc in world. |
| [get_npcs](#get_npcs) | Gets a table of all world npcs. |

## inventory functions
| Function | Description |
|  :----: | ---- |
| [get_item](#get_item_inv) | Gets specified item from inventory. |
| [get_items](#get_items_inv) | Gets a table of all inventory items. |

## player functions
| Function | Description |
|  :----: | ---- |
| [get_clothes](#get_clothes) | Gets a table of all player clothes. |
| [get_tile_pos](#get_tile_pos) | Gets the player's position using tile measurements. |

## tile functions
| Function | Description |
|  :----: | ---- |
| [get_extra](#get_extra) | Gets the extra data of tile. |
| [is_tree_ready](#is_tree_ready) | Gets is the tree on tile is ready to harvest. |

## text_packet functions
| Function | Description |
|  :----: | ---- |
| [load](#load) | Loads text packet. |
| [build](#build) | Gets string of the text packet. |
| [has](#has) | Checks if a specific string is present in text packet. |
| [get](#get) | Gets specific value. |

## variant functions
| Function | Description |
|  :----: | ---- |
| [get_type](#get_type) | Gets variant variable type. |
| [get_float](#get_float) | Gets float value from specified variant. |
| [get_string](#get_string) | Gets string value from specified variant. |
| [get_vec2](#get_vec2) | Gets vec2 value from specified variant. |
| [get_vec3](#get_vec3) | Gets vec3 value from specified variant. |
| [get_uint](#get_uint) | Gets unsigned int value from specified variant. |
| [get_int](#get_int) | Gets intiger value from specified variant. |

## bot_manager functions
| Function | Description |
|  :----: | ---- |
| [add_bot](#add_bot) | Adds a new specified bot. |
| [get_bot](#get_bot) | Gets specified bot. |
| [remove_bot](#remove_bot) | Removes specified bot. |
| [remove_bots](#remove_bots) | Removes all bots. |
| [get_bots](#get_bots) | Gets a table of all bots. |

## item_manager functions
| Function | Description |
|  :----: | ---- |
| [get_item](#get_item) | Gets an specified item. |
| [get_items](#get_items) | Gets a table of all items. |

## other functions
| Function | Description |
|  :----: | ---- |
| [print](#print) | Prints a specified text to GrowBot Console. |
| [create_thread](#create_thread) | Creates a thread. |
| [sleep](#sleep) | Sleeps for a specified amount of time. |
| [send](#sleep) | Sends a webhook message. |
| [edit](#edit) | Edits a webhook message. |

---

<a id="connect"></a>
###  connect function  *([Connection functions](#connection-functions))* 

Connects bot to the growtopia servers.

#### Syntax

```lua
--@return boolean
function connect()
```

#### Parameters

None

#### Return value

Returns true if everything succeded else false.

#### Remarks

This function does not return true if the bot succesfully went online it just returns if the connection to the servers was succesfull but **not the logging** also note that you first need to add the bot to the **bot_manager** before you can call *connect* function you can see that in the example below.

#### Examples

```lua
local bot = bot_manager.add_bot("growid", "pass") -- adds the bot (check add_bot() documentation for more info)
bot:connect() -- calls the connect function for bot
```

---

<a id="disconnect"></a>
###  disconnect function  *([Connection functions](#connection-functions))* 

Disconnects bot from the growtopia servers.

#### Syntax

```lua
--@return boolean
function disconnect()
```

#### Parameters

None

#### Return value

Returns true if everything succeded else false.

#### Remarks

Note that when you call disconnect bot will disconnect and try to connect again if you want to remove it fully remove the bot from bot_manager check examples below

#### Examples

```lua

-- disconnect bot
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:disconnect() -- calls disconnect for bot

-- diconnect bot and remove it
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:disconnect() -- calls disconnect for bot
bot_manager.remove_bot(bot.name) -- removes the bot from bot_manager (check remove_bot() documentation for more info)
```

---

<a id="reconnect"></a>
###  reconnect function  *([Connection functions](#connection-functions))* 

Reconnects bot.

#### Syntax

```lua
function reconnect()
```

#### Parameters

None

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:reconnect() -- reconnects the bot
```

---

<a id="set_pos"></a>
###  set_pos function  *([Bot functions](#bot-functions))*

Sets the bot position to the specified values in parameters.

#### Syntax

```lua
--@param number x 
--@param number y 
function set_pos(x, y)
```

#### Parameters

`x`

the x position that you want the bot to go at.

`y`

the y position that you want the bot to go at.

#### Return value

None

#### Remarks

The function takes a bot position ***float*** that looks like this `1515.0` as parameter not tile position number which looks like this `15` check examples down below. Also note that if you set the position too far away from the current bot position you can get ***banned***.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_pos(1550.0, 2500.0) -- sets bot x position to 1550.0 and y to 2500.0

-- better use case 
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_pos(bot.pos.x + 32.0, bot.pos.y) -- sets the bot position to the current x + 32.0 and to current y this means the bot will simply just move right by one block
```

---

<a id="set_pos_at_tile"></a>
###  set_pos_at_tile function  *([Bot functions](#bot-functions))*

Sets the bot position to the specified tile position values in parameters.

#### Syntax

```lua
--@param number x 
--@param number y 
function set_pos_at_tile(x, y)
```

#### Parameters

`x`

the x tile position that you want the bot to go at.

`y`

the y tile position that you want the bot to go at.

#### Return value

None

#### Remarks

The function takes a bot position ***number*** that looks like this `15` as parameter not position float which looks like this `1534.0` check examples down below. Also note that if you set the position too far away from the current bot position you can get ***banned***. The standart range for x position is from `0` to `100` for y is `0` to `60`

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_pos_at_tile(2, 10) -- sets bot x tile position to 2 and y to 10

-- better use case 
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local bot_pos = bot:get_tile_pos() -- get the current position of bot (check get_tile_pos() documentation for more info)
bot:set_pos_at_tile(bot_pos.x + 1, bot_pos.y) -- sets the bot position to the current x + 1 and to current y this means the bot will simply just move right by one block
```

---

<a id="place_tile"></a>
###  place_tile function  *([Bot functions](#bot-functions))*

Places specified block or background at specific position specified in the parameters.

#### Syntax

```lua
--@param number item_id 
--@param number x 
--@param number y 
function place_tile(item_id, x, y)
```

#### Parameters

`item_id`

the item_id of block or background you want the bot to place.

`x`

the x tile position that you want the bot to place at.

`y`

the y tile position that you want the bot to place at.

#### Return value

None

#### Remarks

Note that if you set the position too far away from the current bot position you can get ***banned***.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:place_tile(4, 2, 10) -- places lava which item_id = 4 and places it to x positon 2 and the y 10

-- better use case
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local bot_pos = bot:get_tile_pos() -- get the current position of bot (check get_tile_pos() documentation for more info)
bot:place_tile(4, bot_pos.x + 1 , bot_pos.y) -- places lava which itemId = 4 and places it to current x positon + 1 and the y to current this means the bot will just place the lava to its right
```

---

<a id="punch_tile"></a>
###  punch_tile function  *([Bot functions](#bot-functions))*

Punches at specified position in the parameters.

#### Syntax

```lua
--@param number x 
--@param number y 
function punch_tile(x, y)
```

#### Parameters

`x`

the x tile position that you want the bot to punch at.

`y`

the y tile position that you want the bot to punch at.

#### Return value

None

#### Remarks

Note that if you set the position too far away from the current bot position you can get ***banned***.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:punch_tile(2, 10) -- punches at x positon 2 and the y 10

-- better use case
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local bot_pos = bot:get_tile_pos() -- get the current position of bot (check get_tile_pos() documentation for more info)
bot:punch_tile(bot_pos.x + 1 , bot_pos.y) -- punches at current x positon + 1 and the y to current bot position this means the bot will punch to its right
```

---

<a id="wrench_tile"></a>
###  wrench_tile function  *([Bot functions](#bot-functions))*

Wrenches at specified position in the parameters.

#### Syntax

```lua
--@param number x 
--@param number y 
function wrench_tile(x, y)
```

#### Parameters

`x`

The x tile position that you want the bot to wrench at.

`y`

The y tile position that you want the bot to wrench at.

#### Return value

None

#### Remarks

Note that if you set the position too far away from the current bot position you can get ***banned***.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:wrench_tile(2, 10) -- wrenches at x positon 2 and the y 10

-- better use case
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local bot_pos = bot:get_tile_pos() -- get the current position of bot (check get_tile_pos() documentation for more info)
bot:wrench_tile(bot_pos.x + 1 , bot_pos.y) -- wrenches at current x positon + 1 and the y to current bot position this means the bot will wrench to its right
```

---

<a id="activate_tile"></a>
###  activate_tile function  *([Bot functions](#bot-functions))*

Activates at specified position in the parameters.

#### Syntax

```lua
--@param number x 
--@param number y 
function activate_tile(x, y)
```

#### Parameters

`x`

The x tile position that you want the bot to activate at.

`y`

The y tile position that you want the bot to activate at.

#### Return value

None

#### Remarks

Note that if you set the position too far away from the current bot position you can get ***banned***. Activating is used for things like checkpoints, portals and similar items in growtopia.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:activate_tile(2, 10) -- activate at x positon 2 and the y 10

-- better use case
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local bot_pos = bot:get_tile_pos() -- get the current position of bot (check get_tile_pos() documentation for more info)
bot:activate_tile(bot_pos.x + 1 , bot_pos.y) -- activate at current x positon + 1 and the y to current bot position this means the bot will wrench to its right 
```

---

<a id="activate_item"></a>
###  activate_item function  *([Bot functions](#bot-functions))*

Activates specified item.

#### Syntax

```lua
--@param number item_id 
function activate_item(item_id)
```

#### Parameters

`item_id`

The item_id of item you can to consume/activate this can be items like milk, blueberry etc.

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:activate_item(868) -- consume milk
```

---

<a id="collect_item"></a>
###  collect_item function  *([Bot functions](#bot-functions))*

Collects specified dropped item by object_id.

#### Syntax

```lua
--@param number object_id 
function collect_item(object_id)
```

#### Parameters

`object_id`

The object_id of item that you want to collect.

#### Return value

None

#### Remarks

Dont forget to check the positions of the item from current position of the bots else you can get ***banned***

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:collect_item(0) -- collect dropped item that has object_id of 0 note need to check for positions else you can get banned easly if the item is like on the other end of the world and you collect it
```

---

<a id="collect_items"></a>
###  collect_items function  *([Bot functions](#bot-functions))*

Collects all items around.

#### Syntax

```lua

function collect_items()
```

#### Parameters

None

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:collect_items() -- collect all dropped items that are around the bot
```

---

<a id="set_bubble"></a>
###  set_bubble function  *([Bot functions](#bot-functions))*

Sets bot bubble to the specified state.

#### Syntax

```lua
--@param number icon_state 
function set_bubble(icon_state)
```

#### Parameters

`icon_state`

The state of the bubble you want the bot theres 3 states `none = 0`, `chatting = 1`, `brb = 2`

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_bubble(1) -- sets bot bubble to chatting
```

---

<a id="say"></a>
###  say function  *([Bot functions](#bot-functions))*

Says specified text to chat.

#### Syntax

```lua
--@param string text 
function say(text)
```

#### Parameters

`text`

The text you want the bot to say in chat

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:say("hello") -- makes the bot say "hello" to chat
```

---

<a id="warp"></a>
###  warp function  *([Bot functions](#bot-functions))*

Goes to the specified world.

#### Syntax

```lua
--@param string world_name 
function warp(world_name)
```

#### Parameters

`world_name`

The world_name you want he bot to go at.

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:warp("start") -- makes the bot go to world "start"
```

---

<a id="exit_world"></a>
###  exit_world function  *([Bot functions](#bot-functions))*

Exits the world.

#### Syntax

```lua
function exit_world()
```

#### Parameters

None

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:exit_world() -- exits world
```

---

<a id="set_mac"></a>
###  set_mac function  *([Bot functions](#bot-functions))*

Sets bot mac address.

#### Syntax

```lua
--@param string mac 
function set_mac(mac)
```

#### Parameters

`mac`

The mac you want the bot to login with.

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_mac("02:2C:6A:1E:59:3D") -- sets the bot mac as "02:2C:6A:1E:59:3D"
```

---

<a id="set_action"></a>
###  set_action function  *([Bot functions](#bot-functions))*

Sets action for bot.

#### Syntax

```lua
--@param string action 
function set_action(action)
```

#### Parameters

`action`

The action you want the bot to display in the bots list this can be like breaking, walking etc.

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_action("breaking") -- sets the bot action as "breaking"
```

---

<a id="find_path"></a>
###  find_path function  *([Bot functions](#bot-functions))*

Find a path to the specified position in the parameters.

#### Syntax

```lua
--@param number x 
--@param number y 
--@param return table
function find_path(x, y)
```

#### Parameters

`x`

The x position you want to find path to.

`y`

The y position you want to find path to.

#### Return value

Returns a table of path positions.

#### Remarks

Note that this function will not move the bot to the position specified you have to make the code to make the bot walk the path returned from this function check examples below.

#### Examples

```lua
function walk_to(bot, x, y)
    for _, pos in pairs(bot:find_path(x, y)) do -- get a table from find_path function and loops the position that are in the table
        bot:set_pos_at_tile(pos.x, pos.y) -- sets the bot position to the next positon in the return table from find_path
        sleep(300) -- delay of 300 miliseconds between each position change (check sleep() documentation for more info)
    end
end

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
walk_to(bot, 10, 12) -- call our own function that will use the path_find function to get table of positions and then loop then to go to the required position
```

---

<a id="get_local_player"></a>
###  get_local_player function  *([Bot functions](#bot-functions))*

Gets the [player structure](#player-structure) of the bot.

#### Syntax

```lua
--@param return table
function get_local_player()
```

#### Parameters

None

#### Return value

Returns a table of player also known as [player structure](#player-structure).

#### Remarks

None

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local player = bot:get_local_player() -- get the bot player structure
print(player.name) -- print the player name also known as the bot name (check print() documentation for more info)
```

---

<a id="get_inventory"></a>
###  get_inventory function  *([Bot functions](#bot-functions))*

Gets the [inventory structure](#inventory-structure) of the bot.

#### Syntax

```lua
--@param return table
function get_inventory()
```

#### Parameters

None

#### Return value

Returns a table of inventory also known as [inventory structure](#inventory-structure).

#### Remarks

None

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local inventory = bot:get_inventory() -- get the bot inventory structure
print(inventory.size) -- print the inventory size also known as backpack size (check print() documentation for more info)
```

---

<a id="send_generic_text"></a>
###  send_generic_text function  *([packet functions](#packet-functions))*

Sends a generic text packet to server.

#### Syntax

```lua
--@param string text
function send_generic_text(text)
```

#### Parameters

`text`

The packet text you want to send.

#### Return value

None

#### Remarks

This is also know as `SendPacket(2, "action|respawn")`.

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:send_generic_text("action|respawn") -- this sends the respawn packet to server which will make the bot respawn
```

---

<a id="send_game_message"></a>
###  send_game_message function  *([packet functions](#packet-functions))*

Sends a game message packet to server.

#### Syntax

```lua
--@param string text
function send_game_message(text)
```

#### Parameters

`text`

The packet text you want to send.

#### Return value

None

#### Remarks

This is also know as `SendPacket(3, "action|quit_to_exit")`.

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:send_game_message("action|quit_to_exit") -- this will send world exit packet wich will make the bot exit world
```

---

<a id="send_game_packet"></a>
###  send_game_packet function  *([packet functions](#packet-functions))*

Sends a game packet to server.

#### Syntax

```lua
--@param table game_packet
function send_game_packet(game_packet)
```

#### Parameters

`game_packet`

The [game_packet](#game_packet-structure) you want to send.

#### Return value

None

#### Remarks

This is also know as `SendPacketRaw`.

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)

local packet = game_packet:new() -- creates new game_packet
packet.type = game_packet_type.set_icon_state -- or just packet.type = 18
packet.net_id = bot:get_local_player().net_id
packet.tile_x = 1 -- icon state

bot:send_game_packet(packet) -- sends the packet to server
```

---

<a id="set_proxy"></a>
###  set_proxy function  *([proxy functions](#proxy-functions))*

Sets the bots proxy.

#### Syntax

```lua
--@param string proxy_ip
--@param number proxy_port
function set_proxy(proxy_ip, proxy_port)
```

#### Parameters

`proxy_ip`

The ip of the proxy like `45.228.16.46`.

`proxy_port`

The port of the proxy like `1080`

#### Return value

None

#### Remarks

None

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_proxy("45.228.16.46", 1080) -- set proxy
```

---

<a id="set_proxy_auth"></a>
###  set_proxy_auth function  *([proxy functions](#proxy-functions))*

Sets the bots proxy authentication.

#### Syntax

```lua
--@param string proxy_username
--@param string proxy_password
function set_proxy_auth(proxy_username, proxy_password)
```

#### Parameters

`proxy_username`

The username of proxy like `kDsls`.

`proxy_password`

The password of proxy like `kfGls`.

#### Return value

None

#### Remarks

Must a proxy first before calling this function check examples below.

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:set_proxy("45.228.16.46", 1080) -- set proxy
bot:set_proxy_auth("kDsls", "kfGls") -- set proxy authentication/login user and pass
```

---

<a id="get_ping"></a>
###  get_ping function  *([proxy functions](#proxy-functions))*

Gets bot ping.

#### Syntax

```lua
--@param return number
function get_ping()
```

#### Parameters

None

#### Return value

Returns integer of the ping.

#### Remarks

None

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
ping = bot:get_ping() -- get the ping
print(ping) -- print ping
```

---

<a id="get_proxy_reply"></a>
###  get_proxy_reply function  *([proxy functions](#proxy-functions))*

Gets bot proxy reply.

#### Syntax

```lua
--@param return number
function get_proxy_reply()
```

#### Parameters

None

#### Return value

Returns a proxy reply code.

#### Remarks

None

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
reply = bot:get_proxy_reply() -- get the reply
print(reply) -- print reply
```

---

<a id="get_proxy_string"></a>
###  get_proxy_string function  *([proxy functions](#proxy-functions))*

Gets bot proxy string.

#### Syntax

```lua
--@param return string
function get_proxy_string()
```

#### Parameters

None

#### Return value

Returns a proxy in string format ip:port:user:pass.

#### Remarks

None

#### Examples

```lua

local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
proxy = bot:get_proxy_string() -- get the proxy string
print(proxy) -- print proxy string
```

---

<a id="remove_callback"></a>
###  remove_callback function  *([callback functions](#callback-functions))*

Removes callback by the specified name in the parameter.

#### Syntax

```lua
--@param string callback_name
function remove_callback(callback_name)
```

#### Parameters

`callback_name`

The name of the callback you want to remove.

#### Return value

None

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:remove_callback("callback_name") -- removes callback with the specified name
```

---

<a id="has_callback"></a>
###  has_callback function  *([callback functions](#callback-functions))*

Checks if that callback exists by the passed name in parameter.

#### Syntax

```lua
--@param string callback_name
--@return boolean
function has_callback(callback_name)
```

#### Parameters

`callback_name`

The name of the callback you want to check if it exists.

#### Return value

Returns true if the callback exists false if not.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
does_exist = bot:has_callback("callback_name") -- removes callback with the specified name
print(does_exist) -- print the result
```

---

<a id="add_game_message_callback"></a>
###  add_game_message_callback function  *([callback functions](#callback-functions))*

Adds game message callback.

#### Syntax

```lua
--@param string callback_name
--@param function callback_function
function add_game_message_callback(callback_name, callback_function)
```

#### Parameters

`callback_name`

The name of the callback.

`callback_function`

The function that gets called after in the callback.

#### Return value

None

#### Remarks

Note that u can't use [sleep](#sleep) inside the callback function but u can use [create_thread](#create_thread) check examples below.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_game_message_callback( -- add the callback
  "callback name", 
  function(bot, packet)
    local action = packet:get("action") --(check get() documentation for more info)
    if action == "log" then
      print(string.format("%s: console log \"%s\"", bot.name, packet:get("msg")))
    end
  end
)

-- usage if you need to have sleep inside you callback
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)

function callback_thread()
    sleep(200) -- here you can use sleep and this line of code will sleep the program for 200 miliseconds (check sleep() documentation for more info)
    print("hello from callback thread")
end

bot:add_game_message_callback( -- add the callback
  "callback name", 
  function(bot, packet)
      create_thread(callback_thread)
  end
)

```

---

<a id="add_game_packet_callback"></a>
###  add_game_packet_callback function  *([callback functions](#callback-functions))*

Adds game packet callback.

#### Syntax

```lua
--@param string callback_name
--@param function callback_function
function add_game_packet_callback(callback_name, callback_function)
```

#### Parameters

`callback_name`

The name of the callback.

`callback_function`

The function that gets called after in the callback.

#### Return value

None

#### Remarks

Note that u can't use [sleep](#sleep) inside the callback function but u can use [create_thread](#create_thread) check examples below.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_game_packet_callback( -- add the callback
  "callback name", 
  function(bot, packet)
     print(bot.name)
  end
)

-- usage if you need to have sleep inside you callback
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)

function callback_thread()
    sleep(200) -- here you can use sleep and this line of code will sleep the program for 200 miliseconds (check sleep() documentation for more info)
    print("hello from callback thread")
end

bot:add_game_packet_callback( -- add the callback
  "callback name", 
  function(bot, packet)
      create_thread(callback_thread)
  end
)

```

---

<a id="add_function_call_callback"></a>
###  add_function_call_callback function  *([callback functions](#callback-functions))*

Adds function call callback.

#### Syntax

```lua
--@param string callback_name
--@param function callback_function
function add_function_call_callback(callback_name, callback_function)
```

#### Parameters

`callback_name`

The name of the callback.

`callback_function`

The function that gets called after in the callback.

#### Return value

None

#### Remarks

Note that u can't use [sleep](#sleep) inside the callback function but u can use [create_thread](#create_thread) check examples below.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
     if var_list[0]:get_string() == "OnDialogRequest" then
      print("dialog text: " .. var_list[1]:get_string()) --(check get_string() documentation for more info)
     end
  end
)

-- usage if you need to have sleep inside you callback
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)

function callback_thread()
    sleep(200) -- here you can use sleep and this line of code will sleep the program for 200 miliseconds (check sleep() documentation for more info)
    print("hello from callback thread")
end

bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, variant, net_id, delay)
      create_thread(callback_thread)
  end
)
```

---

<a id="add_track_packet_callback"></a>
###  add_track_packet_callback function  *([callback functions](#callback-functions))*

Adds track packet callback.

#### Syntax

```lua
--@param string callback_name
--@param function callback_function
function add_track_packet_callback(callback_name, callback_function)
```

#### Parameters

`callback_name`

The name of the callback.

`callback_function`

The function that gets called after in the callback.

#### Return value

None

#### Remarks

Note that u can't use [sleep](#sleep) inside the callback function but u can use [create_thread](#create_thread) check examples below.

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_track_packet_callback( -- add the callback
  "callback name", 
  function(bot, packet)
     print(bot.name)
  end
)

-- usage if you need to have sleep inside you callback
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)

function callback_thread()
    sleep(200) -- here you can use sleep and this line of code will sleep the program for 200 miliseconds (check sleep() documentation for more info)
    print("hello from callback thread")
end

bot:add_track_packet_callback( -- add the callback
  "callback name", 
  function(bot, packet)
      create_thread(callback_thread)
  end
)
```

---

<a id="get_world"></a>
###  get_world function  *([world functions](#world-functions))*

Gets [world structure](#world-structure) bot is currently in.

#### Syntax

```lua
--@return table
function get_world()
```

#### Parameters

None

#### Return value

Returns a table of [world structure](#world-structure).

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get the world
print(world.name) -- print the name of the world bot is currently in
```

---

<a id="get_tile"></a>
###  get_tile function  *([world functions](#world-functions))*

Gets [tile](#tile-structure) from the specified position.

#### Syntax

```lua
--@param number x
--@param number y
--@return table
function get_tile(x, y)
```

#### Parameters

`x`

The x position of the tile you want to get.

`y`

The y position of the tile you want to get.

#### Return value

Returns a table of [tile structure](#tile-structure).

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get the world
local tile = world:get_tile(0, 0) -- get the tile at pos x = 0 and y = 0
print(tile.foreground) -- print the tile foreground item_id
```

---

<a id="get_tiles"></a>
###  get_tiles function  *([world functions](#world-functions))*

Gets table of all [tiles](#tile-structure) in the world.

#### Syntax

```lua
--@return table
function get_tiles()
```

#### Parameters

None

#### Return value

Returns a table of all tiles in the world.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local tiles = world:get_tiles() -- get all the tiles in the world

for _, tile in pairs(tiles) do 
  print(tile.foreground) -- prints all the tiles foreground item ids in the world
end
```

---

<a id="get_world_object"></a>
###  get_world_object function  *([world functions](#world-functions))*

Gets table of the specified [world object structure](#world_object-structure) in the world.

#### Syntax

```lua
--@param number object_id
--@return table
function get_world_object(object_id)
```

#### Parameters

`object_id`

The object_id of and object u want to get.

#### Return value

Returns a table of the [world object structure](#world_object-structure).

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local world_object = world:get_world_object(0) -- get the world object with the object_id of 0
print(world_object.item_id) -- print the dropped item_id
```

---

<a id="get_world_objects"></a>
###  get_world_objects function  *([world functions](#world-functions))*

Gets table of all the [world objects](#world_object-structure) in the world.

#### Syntax

```lua
--@return table
function get_world_objects()
```

#### Parameters

None

#### Return value

Returns a table of all the world objects.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local world_objects = world:get_world_objects() -- get all the objects in the world also know as dropped items

for _, world_object in pairs(world_objects) do 
  print(world_object.item_id) -- prints all the world_object item ids in the world
end
```

---

<a id="get_player"></a>
###  get_player function  *([world functions](#world-functions))*

Gets table of the specified [player](#player-structure) in the world.

#### Syntax

```lua
--@param number net_id
--@return table
function get_player(net_id)
```

#### Parameters

`net_id`

The net_id of an player u want to get.

#### Return value

Returns a table of the [player structure](#player-structure).

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local player = world:get_player(0) -- get the player with the net_id of 0
print(player.name) -- print the player name
```

---

<a id="get_players"></a>
###  get_players function  *([world functions](#world-functions))*

Gets table of all the [players](#player-structure) in the world.

#### Syntax

```lua
--@return table
function get_players()
```

#### Parameters

None

#### Return value

Returns a table of all the players.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local players = world:get_players() -- get all the players in the world

for _, player in pairs(players) do 
  print(player.name) -- prints all the player names in the world
end
```

---

<a id="get_npc"></a>
###  get_npc function  *([world functions](#world-functions))*

Gets table of the specified [npc](#npc-structure)  in the world.

#### Syntax

```lua
--@param number npc_id
--@return table
function get_npc(npc_id)
```

#### Parameters

`npc_id`

The npc_id of an [npc](#npc-structure) u want to get.

#### Return value

Returns a table of the [npc](#npc-structure)  structure.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local npc = world:get_npc(0) -- get the npc with the npc_id of 0
print(npc.type) -- print the npc type
```

---

<a id="get_npcs"></a>
###  get_npcs function  *([world functions](#world-functions))*

Gets table of all the [npcs](#npc-structure) in the world.

#### Syntax

```lua
--@return table
function get_npcs()
```

#### Parameters

None

#### Return value

Returns a table of all the [npcs](#npc-structure) in the world.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get world structure
local npcs = world:get_npcs() -- get all the npcs in the world

for _, npc in pairs(npcs) do 
  print(npc.type) -- prints all the npc types in world
end
```

---

<a id="get_item_inv"></a>
###  get_item function  *([inventory functions](#inventory-functions))*

Gets table of the specified [item](#inventory_item-structure) from the inventory.

#### Syntax

```lua
--@param number item_id
--@return table
function get_item(item_id)
```

#### Parameters

`item_id`

The item_id of an item u want to get from inventory.

#### Return value

Returns a table of the of [item structure](#inventory_item-structure).

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local inventory = bot:get_inventory() -- get inventory structure
local inventory_item = inventory:get_item(2) -- get the item from inventory that is item_id 2
print(inventory_item.count) -- print the item count
```

---

<a id="get_items_inv"></a>
###  get_items function  *([inventory functions](#inventory-functions))*

Gets table of all the inventory [items](#inventory_item-structure).

#### Syntax

```lua
--@return table
function get_items()
```

#### Parameters

None

#### Return value

Returns a table of all the [items](#inventory_item-structure) in inventory.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local inventory = bot:get_inventory() -- get inventory structure
local inventory_items = inventory:get_items() -- get all the invenotry items

for _, inventory_item in pairs(inventory_items) do 
  print(inventory_item.item_id) -- prints all the item_id's that are in inventory
end
```

---


<a id="get_clothes"></a>
###  get_clothes function  *([player functions](#player-functions))*

Gets table of [clothes](#clothes-structure) structure that [player](#player-structure) is wearing.

#### Syntax

```lua
--@return table
function get_clothes()
```

#### Parameters

None

#### Return value

Returns a table of all [clothes](#clothes-structure) the [player](#player-structure) is wearing.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local player = bot:get_local_player() -- get player structure
local clothes = player:get_clothes() -- get all clothes that player is wearing

print(clothes.hat) -- prints the hat item_id the player is wearing
```

---

<a id="get_tile_pos"></a>
###  get_tile_pos function  *([player functions](#player-functions))*

Gets [vec2i](#vec2i-structure) of tile position the player is located at.

#### Syntax

```lua
--@return vec2i
function get_tile_pos()
```

#### Parameters

None

#### Return value

Returns a [vec2i](#vec2i-structure) of tile position the player is located at.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local player = bot:get_local_player() -- get player structure
local position = player:get_tile_pos() -- gets the position in tile

print(position.x) -- print the x position
```

---

<a id="get_extra"></a>
###  get_extra function  *([tile functions](#tile-functions))*

Gets [tile_extra](#tile_extra-structure) type of the tile.

#### Syntax

```lua
--@return table
function get_extra()
```

#### Parameters

None

#### Return value

Returns [tile_extra](#tile_extra-structure) type of the tile.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get the world structure
local tile = world:get_tile(0, 0) -- get the first tile in the world
local tile_extra = tile:get_extra() -- gets the tile extra data

print(tile_extra.type) -- print tile extra data type
```

---

<a id="is_tree_ready"></a>
###  is_tree_ready function  *([tile functions](#tile-functions))*

Checks if the tree on tile is ready or not.

#### Syntax

```lua
--@return boolean
function is_tree_ready()
```

#### Parameters

None

#### Return value

Returns true if the tree on the tile is ready for harvest if no false.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local world = bot:get_world() -- get the world structure
local tile = world:get_tile(0, 0) -- get the first tile in the world

local is_ready = tile:is_tree_ready()

if is_ready then
  print("tree is ready for harvest")
else
  print("tree is not ready for harvest")
end
```

---

<a id="load"></a>
###  load function  *([text_packet functions](#text_packet-functions))*

Loads text_packet from a string.

#### Syntax

```lua
--@param string text
function load(text)
```

#### Parameters

`text`

Text of the packet u want to load into the text_packet

#### Return value

None

#### Remarks

None

#### Examples

```lua
packet = text_packet:new()
packet:load("your|text")
```

---

<a id="build"></a>
###  build function  *([text_packet functions](#text_packet-functions))*

Makes a text_packet into a string.

#### Syntax

```lua
--@param table text_packet
--@return string
function build(text_packet)
```

#### Parameters

`text_packet`

The text packet that you want to get as string.

#### Return value

Returns a string of the packet.

#### Remarks

None

#### Examples

```lua
packet = text_packet:new()
packet:load("your|text")

packet_string = packet:build()
print(packet_string)
```

---

<a id="has"></a>
###  has function  *([text_packet functions](#text_packet-functions))*

Checks if text_packet has the value specified.

#### Syntax

```lua
--@param string text
--@return boolean
function has(text)
```

#### Parameters

`text`

The text that u want to check if exists in text_packet.

#### Return value

Returns true if theres the text else returns false.

#### Remarks

None

#### Examples

```lua
packet = text_packet:new()
packet:load("your|text")

does_exist = packet:has("your")
print(does_exist)
```

---

<a id="get"></a>
###  get function  *([text_packet functions](#text_packet-functions))*

Find value by the specified indentifire in parameter.

#### Syntax

```lua
--@param string text
--@return string
function get(text)
```

#### Parameters

`text`

The indentifier of the value u want to get

#### Return value

Returns a string of the value gotten.

#### Remarks

None

#### Examples

```lua
packet = text_packet:new()
packet:load("your|text")

value = packet:get("your")
print(value)
```

---

<a id="get_type"></a>
###  get_type function  *([variant functions](#variant-functions))*

Get the type of variant variable.

#### Syntax

```lua
--@return number
function get_type()
```

#### Parameters

None

#### Return value

Returns the type.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local type = var_list[1]:get_type() -- get the type
      print(type) -- print out the type
     end
  end
)
```

---

<a id="get_float"></a>
###  get_float function  *([variant functions](#variant-functions))*

Get float value of variant variable.

#### Syntax

```lua
--@return number
function get_float()
```

#### Parameters

None

#### Return value

Returns the float value.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local float_value = var_list[1]:get_float() -- get the float from var_list[1]
      print(float_value) -- print out the value we got from get_float function
     end
  end
)
```

---

<a id="get_string"></a>
###  get_string function  *([variant functions](#variant-functions))*

Get string value of variant variable.

#### Syntax

```lua
--@return string
function get_string()
```

#### Parameters

None

#### Return value

Returns the string value.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local string = var_list[0]:get_string() -- get the string from var_list[0]
      print(string) -- print out the string we got from get_string function
     end
  end
)
```

---

<a id="get_vec2"></a>
###  get_vec2 function  *([variant functions](#variant-functions))*

Get vec2f value of variant variable.

#### Syntax

```lua
--@return table
function get_vec2()
```

#### Parameters

None

#### Return value

Returns the [vec2f](#vec2f-structure) value.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local vec2f = var_list[2]:get_vec2() -- get the vec2f from var_list[2]
      print(vec2f.x) -- print out the x value of vec we got from get_vec2 function
     end
  end
)
```

---

<a id="get_vec3"></a>
###  get_vec3 function  *([variant functions](#variant-functions))*

Get vec3f value of variant variable.

#### Syntax

```lua
--@return table
function get_vec3()
```

#### Parameters

None

#### Return value

Returns the [vec3f](#vec3f-structure) value.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local vec3f = var_list[2]:get_vec3() -- get the vec3f from var_list[2]
      print(vec3f.z) -- print out the z value of vec we got from get_vec3 function
     end
  end
)
```

---

<a id="get_uint"></a>
###  get_uint function  *([variant functions](#variant-functions))*

Get unsigned int value of variant variable.

#### Syntax

```lua
--@return number
function get_uint()
```

#### Parameters

None

#### Return value

Returns the unsigned int value.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local uint = var_list[2]:get_uint() -- get the number (uint) from var_list[2]
      print(uint) -- print out the number we got from get_uint function
     end
  end
)
```

---

<a id="get_int"></a>
###  get_int function  *([variant functions](#variant-functions))*

Get int value of variant variable.

#### Syntax

```lua
--@return number
function get_int()
```

#### Parameters

None

#### Return value

Returns the int value.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local int = var_list[2]:get_int() -- get the number (int) from var_list[2]
      print(int) -- print out the number we got from get_int function
     end
  end
)
```

---

<a id="add_bot"></a>
###  add_bot function  *([bot_manager functions](#bot_manager-functions))*

Add a new [bot](#bot-structure) to the bot_manager.

#### Syntax

```lua
--@param string growid
--@param string pass
--@return table
function add_bot(growid, pass)
```

#### Parameters

`growid`

The growid of the bot you want to add or the guest growid.

`pass`

The password of the account.

#### Return value

Returns [bot](#bot-structure) structure.

#### Remarks

None

#### Examples

```lua
--add bot with growid and pass
local bot = bot_manager.add_bot("growid", "pass")

--add bot with guest growid
local bot = bot_manager.add_bot("growid")
```

---

<a id="get_bot"></a>
###  get_bot function  *([bot_manager functions](#bot_manager-functions))*

Get a [bot](#bot-structure) from the bot_manager structure.

#### Syntax

```lua
--@param string growid
--@return table
function get_bot(growid)
```

#### Parameters

`growid`

The growid of the bot you want to get.

#### Return value

Returns [bot](#bot-structure) structure.

#### Remarks

None

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
```

---


<a id="remove_bot"></a>
###  remove_bot function  *([bot_manager functions](#bot_manager-functions))*

Remove a bot from the bot_manager structure.

#### Syntax

```lua
--@param string growid
function remove_bot(growid)
```

#### Parameters

`growid`

The growid of the bot you want to remove.

#### Return value

None

#### Remarks

None

#### Examples

```lua
bot_manager.remove_bot("growid")
```

---

<a id="remove_bots"></a>
###  remove_bots function  *([bot_manager functions](#bot_manager-functions))*

Removes all bots from the bot_manager structure.

#### Syntax

```lua
function remove_bots()
```

#### Parameters

None

#### Return value

None

#### Remarks

None

#### Examples

```lua
bot_manager.remove_bots()
```

---

<a id="get_bots"></a>
###  get_bots function  *([bot_manager functions](#bot_manager-functions))*

Gets all [bots](#bot-structure) from the bot_manager structure.

#### Syntax

```lua
--@return table
function get_bots()
```

#### Parameters

None

#### Return value

Returns a table with all [bots](#bot-structure).

#### Remarks

None

#### Examples

```lua
local bots = bot_manager.get_bots()

for _, bot in pairs(bots) do
  print(bot.name) -- print all the bots names
end
```

---

<a id="get_item"></a>
###  get_item function  *([item_manager functions](#item_manager-functions))*

Gets [item](#item-structure) from the item_manager structure.

#### Syntax

```lua
--@param item_id
--@return table
function get_item(item_id)
```

#### Parameters

`item_id`

The item_id of [item](#item-structure) you want to get.

#### Return value

Returns a table of [item structure](#item-structure).

#### Remarks

None

#### Examples

```lua
local item = item_manager.get_item(2)

print(item.name) -- prints out the item name which is Dirt
```

---

<a id="get_items"></a>
###  get_items function  *([item_manager functions](#item_manager-functions))*

Gets a table of all [items](#item-structure) from the item_manager structure.

#### Syntax

```lua
--@return table
function get_items()
```

#### Parameters

None

#### Return value

Returns a table with all items from the item_manager.

#### Remarks

None

#### Examples

```lua
local items = item_manager.get_items()

for _, item in pairs(items) do
  print(item.name) -- print all item names
end
```

---


<a id="print"></a>
###  print function  *([other functions](#other-functions))*

Prints a specified text in parameter to the GrowBot Console.

#### Syntax

```lua
--@param string text
function print(text)
```

#### Parameters

`text`

The text you want to print in GrowBot Console.

#### Return value

None

#### Remarks

None

#### Examples

```lua
print("hello world") -- prints "hello world" to GrowBot Console
```

---

<a id="create_thread"></a>
###  create_thread function  *([other functions](#other-functions))*

Creates a thread and runs the specified function in a thread.

#### Syntax

```lua
--@param function thread_func
function create_thread(thread_func)
```

#### Parameters

`thread_func`

The function that u want to run in thread.

#### Return value

None

#### Remarks

None

#### Examples

```lua

function hello_world()
  print("Hello") -- prints "Hello" to the GrowBot Console
end

create_thread(hello_world) -- starts a thread and runs the hello_world world function which prints out "Hello"
```

---

<a id="sleep"></a>
###  sleep function  *([other functions](#other-functions))*

Sleeps the program for certain amount of time specified in the parameter.

#### Syntax

```lua
--@param number miliseconds
function sleep(miliseconds)
```

#### Parameters

`miliseconds`

The time in miliseconds u want the program to sleep for.

#### Return value

None

#### Remarks

None

#### Examples

```lua
print("hello") -- prints "hello"
sleep(1000) -- sleeps for 1000 miliseconds
print("hello") -- prints "hello" after 1000 miliseconds have passed
```

---

<a id="send"></a>
###  send function  *([other functions](#other-functions))*

Sends a webhook message to the specified webhook.

#### Syntax

```lua
--@param string url
--@param string content
function send(url, content)
```

#### Parameters

`url`

The url/link for the webhook you want to send the message to.

`content`

Content of the message.

#### Return value

None

#### Remarks

Check out discord webhook documentation [here](https://discord.com/developers/docs/resources/webhook#execute-webhook-jsonform-params)

#### Examples

```lua

local url = 'your webhook url/link here'
local message = '{"content":"hello"}'

webhook.send(url, message) -- sends hello world message to the webhook
```

---

<a id="edit"></a>
###  edit function  *([other functions](#other-functions))*

Edits a webhook message to the specified webhook.

#### Syntax

```lua
--@param string url
--@param string message_id
--@param string content
function edit(url, message_id, content)
```

#### Parameters

`url`

The url/link for the webhook you want to send the message to.

`message_id`

The message_id you want to edit message of.

`content`

Content of the message.

#### Return value

None

#### Remarks

Check out discord webhook documentation [here](https://discord.com/developers/docs/resources/webhook#execute-webhook-jsonform-params)

#### Examples

```lua

local url = 'your webhook url/link here'
local message_id = 'your message id here'
local message = '{"content":"hello"}'

webhook.edit(url, message_id, message) -- edits the message you specified
```

---

# Structures

This section provides documentation on GrowBot structures. Below, you will find tables that represent all the structures available in the GrowBot Lua API.

- Quick links
  - [bot structure](#bot-structure) 
  - [world structure](#world-structure)
  - [inventory structure](#inventory-structure)
  - [inventory_item structure](#inventory_item-structure)
  - [player structure](#player-structure)
  - [tile structure](#tile-structure)
  - [tile_extra structure](#tile_extra-structure)
  - [world_object structure](#world_object-structure)
  - [game_packet structure](#game_packet-structure)
  - [vec2f structure](#vec2f-structure)
  - [vec3f structure](#vec3f-structure)
  - [vec2i structure](#vec2i-structure)
  - [item structure](#item-structure)
  - [clothes structure](#clothes-structure)
  - [npc structure](#npc-structure)

---

## bot structure

The bot structure represents a bot.

Type | Name | Description |
:----: |  :----: | ---- |
number | status | This field stores the current [bot_status](#bot_status-enum) of the bot like connected, disconnected etc. |
string | name | This field stores the name of the bot. |
string | name | This field stores the password of the bot. |
number | gems | This field stores the gems amount the bot has. |
number | level | This field stores the current level of the bot. |

This structure contains functions presented below.
  - [set_pos](#set_pos)
  - [set_pos_at_tile](#set_pos_at_tile)
  - [place_tile](#place_tile)
  - [punch_tile](#punch_tile)
  - [wrench_tile](#wrench_tile)
  - [activate_tile](#activate_tile)
  - [activate_item](#activate_item) 
  - [collect_item](#collect_item)
  - [collect_items](#collect_items)
  - [set_bubble](#set_bubble)
  - [say](#say)
  - [warp](#warp)
  - [exit_world](#exit_world)
  - [set_mac](#set_mac)
  - [set_action](#set_action)
  - [find_path](#find_path)
  - [get_local_player](#get_local_player)
  - [get_inventory](#get_inventory)

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
-- bot = bot structure
print(bot.name) -- print out the bot name
print(bot.level) -- print out the bot level
print(bot.gems) -- print out the bot gems
```

---

## world structure

The world structure represents the current world in which the bot is located.

Type | Name | Description |
:----: |  :----: | ---- |
string | name | This field stores the name of the world in which the bot is currently located. |
[vec2i](#vec2i-structure) | size | This field stores the dimensions of the world. It represents the width and height of the world, specified as a two-dimensional vector of integers. The size indicates the extent of the world in terms of tiles or blocks. The world standard size is `x = 100` and `y = 60`, |

This structure contains functions presented below.
  - [get_world](#get_world)
  - [get_tile](#get_tile)
  - [get_tiles](#get_tiles)
  - [get_world_object](#get_world_object)
  - [get_world_objects](#get_world_objects)
  - [get_player](#get_player)
  - [get_players](#get_players)
  - [get_npc](#get_npc)
  - [get_npcs](#get_npcs)


#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local world = bot:get_world()
-- world = world structure
print(world.name) -- prints out the world name the bot is currently in
print(world.size.x) -- prints out the x size of the world also known as world width/lenght
print(world.size.y) -- prints out the y size of the world also known as world height
```

---

## inventory structure

The inventory structure represents an player's also known as bot's inventory within the game.

Type | Name | Description |
:----: |  :----: | ---- |
number | size | This field stores the size of backpack. |


This structure contains functions presented below.
  - [get_item](#get_item_inv)
  - [get_items](#get_items_inv)

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local inventory = bot:get_inventory()
-- inventory = inventory structure
print(inventory.size) -- prints out the inventory size

for _, inventory_item in pairs(inventory:get_items()) do -- loops all items in inventory and prints their names
  -- inventory_item = inventory_item structure
  local item = item_manager.get_item(inventory_item.item_id) -- gets the item structure from item manager
  -- item = item structure
  print(item.name) -- prints out the item name  
end
```

---

## inventory_item structure

The inventory_item structure represents an item in a player's also known as bot's inventory within the game.

Type | Name | Description |
:----: |  :----: | ---- |
number | item_id | This field stores the item_id, which serves as a unique identifier for the item in the game. |
number | count | This field stores the count of the item, indicating the quantity of that particular item present in the player's inventory. |

This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local inventory = bot:get_inventory() 
-- inventory = inventory structure
local inventory_item = inventory:get_item(2) -- get dirt item
-- inventory_item = inventory_item structure
print(inventory_item.count) -- print out the count of item in inventory in this case the dirt amount in inventory
```

---

## player structure

The player structure represents a player in the game.

Type | Name | Description |
:----: |  :----: | ---- |
string | name | This field stores the player's name, commonly referred to as the GrowID or guest GrowID. |
number | net_id | This field stores the net_id of the player, indicating the unique identifier for the player in world. |
number | user_id | This field stores the user_id of the player, serving as the unique identifier for the player's account. |
[vec2f](#vec2f-structure) | pos | This field stores the player's position within the world, specifying the coordinates where the player is located. The position is represented using a two-dimensional vector with floating-point values, denoting the player's X and Y coordinates. |

This structure contains functions presented below.
  - [get_clothes](#get_clothes)
  - [get_tile_pos](#get_tile_pos)

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local world = bot:get_world()

for _, player in pairs(world:get_players()) do -- prints all player names in the world
  -- player = player structure
  print(player.name)
end
```

---

## tile structure

The tile structure represents a block, background, or a combination of both within a world.

Type | Name | Description |
:----: |  :----: | ---- |
number | index | This field stores the tile index, serving as unique identifier of the tile. |
[vec2i](#vec2i-structure) | pos | This field stores the position of the tile, indicating its coordinates within the world. The position is represented by numeric values, such as `x = 10` and `y = 5.` Typically, the maximum values for x and y depend on the size of the world, but a common range is `x <= 100` and `y <= 60.`|
number | foreground | This field holds the foreground itemId, representing the item identifier associated with the block of the tile. It commonly refers to items like `Lava` with an itemId of `4`.|
number | background | This field holds the background itemId, representing the item identifier associated with the background of the tile. It commonly refers to items like `Cave Background` with an itemId of `14`.|
number  | flags  | this field stores additional flags associated with the tile, indicating further attributes or properties. These flags provide information about the tile's behavior or characteristics, such as the presence of fire, the enabled status of a jammer, or other relevant features. |

This structure contains functions presented below.
  - [get_extra](#get_extra)

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local world = bot:get_world()

for _, tile in pairs(world:get_tiles()) do -- prints all tile foreground item_id's in the world
  -- tile = tile structure
  print(tile.foreground)
end
```

---

## tile_extra structure

The tile_extra structure represents the additional data associated with a [tile](#tile-structure).

Type | Name | Description |
:----: |  :----: | ---- |
number | type | This field stores the type of tile_extra. |


This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local world = bot:get_world()

for _, tile in pairs(world:get_tiles()) do -- prints all tile extra types in the world
  -- tile = tile structure
  local tile_extra = tile:get_extra()
  -- tile_extra = tile_extra structure
  print(tile_extra.type)
end
```

---

## world_object structure

The world_object structure represents a dropped item within the world and has few fields that are documented below.

Type | Name | Description |
:----: |  :----: | ---- |
number | item_id | This field stores the item id of the world_object, often referred to as the item id of a dropped item within the world.
 [vec2f](#vec2f-structure) | pos | This field stores the position of the world_object, indicating the coordinates where the dropped item is located within the world.
 number | count | This field stores the count of the world_object, representing the quantity of the dropped item within the world.
 number | flags | This field stores the flags of the world_object, denoting additional attributes or properties associated with the dropped item within the world.
 number | object_id | This field stores the object id of the world_object, representing a unique identifier assigned to the dropped item within the world.

This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local world = bot:get_world()

for _, object in pairs(world:get_objects()) do -- prints all dropped items names in the world
  -- object = world_object structure
  local item = item_manager.get_item(object.item_id) -- gets the item structure from item manager
  -- item = item structure
  print(item.name) -- prints out the item name  
end
```

---

## game_packet structure

The game_packet structure represents a game packet used in the Growtopia game, which is sent to the server and contains various values documented below.

Type | Name | Description |
:----: |  :----: | ---- |
| number | type | This field stores the [game_packet_type](#game_packet_type-enum) of game_packet. |
| number | byte1 | This field stores the byte1 also known as objtype, punchid, or npctype.  |
| number | byte2 | This field stores the byte2 also known as count1, jump_count, build_range, npc_id, or lost_item_count. |
| number | byte3 | This field stores the byte3 also known as count2, count, animation_type, punch_range, npc_action, particle_id, gained_item_count, dice_result, or fruit_count. |
| number | net_id | This field stores the net_id also known as netid, player_flags, game_packet_type, effect_flags_check, object_change_type, or particle_emitter_id. |
| number | secondary_value | This field stores the secondary_value also known as item, ping_hash, item_netid, pupil_color, or tiles_length. |
| number | flags | This field stores the flags also known as packet_flags. |
| number | float1 | This field stores the float1 also known as float_var, struct_flags, int_var, water_speed, or obj_alt_count. |
| number | main_value | This field stores the main_values also known as int_data, ping_item, elapsed_ms, delay, tile_damage, item_id, item_speed, effect_flags, object_id, hash, verify_pos, client_hack_type. |
| [vec2f](#vec2f-structure) | vec1 | This field stores the vec1 also known as vec or (vec_x, vec_y). |
| [vec2f](#vec2f-structure) | vec2 | This field stores the vec1 also known as vec2 or (vec2_x, vec2_y). |
| number | float2 | This field stores the float2 also known as particle_time.  |
| number | tile_x | This field stores the tile_x also known as int_x, state1. |
| number | tile_y | This field stores the tile_y also known as int_y, state2. |
| number | extra_data_size | This field stores the extra_data_size also known as data_size. |


This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)

local packet = game_packet:new() -- creates new game_packet
packet.type = game_packet_type.set_icon_state -- or just packet.type = 18
packet.net_id = bot:get_local_player().net_id
packet.tile_x = 1 -- icon state

bot:send_game_packet(packet) -- sends the packet to server
```

---

## vec2f structure

The vec2f structure represents a two-dimensional vector with an x and y coordinate. It is used to store floating-point values for both the x and y coordinates. The 'x' field specifically stores the x-coordinate value as a float, while the 'y' field stores the y-coordinate value as a float.

Type | Name | Description |
:----: |  :----: | ---- |
| number | x | This field stores the x-coordinate value (floating-point number or float, e.g., `50.0`). |
| number | y | This field stores the y-coordinate value (floating-point number or float, e.g., `50.0`). |



This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local player = bot:get_local_player() -- get player structure
local position = player.pos -- gets the position in tile
-- position = vec2f structure
print(position.x) -- print the x position
print(position.y) -- print the y position
```

---


## vec3f structure

The vec3f structure represents a three-dimensional vector with x, y, and z coordinates. It is used to store numerical values for each coordinate. The 'x' field specifically stores the x-coordinate value, which can be represented as a floating-point number or simply as a float, such as `50.0`. Similarly, the 'y' and 'z' fields store the y-coordinate and z-coordinate values, respectively, following the same representation.

Type | Name | Description |
:----: |  :----: | ---- |
| number | x | This field stores the x-coordinate value (floating-point number or float, e.g., `55.0`). |
| number | y | This field stores the y-coordinate value (floating-point number or float, e.g., `55.0`). |
| number | z | This field stores the z-coordinate value (floating-point number or float, e.g., `55.0`). |


This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
bot:add_function_call_callback( -- add the callback
  "callback name", 
  function(bot, var_list, net_id, delay)
      local vec3f = var_list[2]:get_vec3() -- get the vec3f from var_list[2]
      -- vec3f = vec3f structure
      print(vec3f.z) -- print out the z value of vec we got from get_vec3 function
      print(vec3f.x) -- print out the x value of vec we got from get_vec3 function
      print(vec3f.y) -- print out the y value of vec we got from get_vec3 function
     end
  end
)
```

---


## vec2i structure

The vec2i structure represents a two-dimensional vector with an x and y coordinate. It is used to store integer values for both the x and y coordinates. The 'x' field specifically stores the x-coordinate value as a number, such as `100`. Similarly, the 'y' field stores the y-coordinate value as a number, also illustrated by the example value of `100`.

Type | Name | Description |
:----: |  :----: | ---- |
| number | x | This field stores the x-coordinate value (integer, e.g., `100`). |
| number | y | This field stores the x-coordinate value (integer, e.g., `100`). |


This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local player = bot:get_local_player() -- get player structure
local position = player:get_tile_pos() -- gets the position in tile
-- position = vec2i structure

print(position.x) -- print the x position
print(position.y) -- print the y position
```

---

## item structure

The item structure represents an item in game. It contains several fields that provide information about the item. The 'id' field serves as a unique identifier, commonly known as itemId. For example, the item `Lava` has an itemId of `4`. The 'name' field stores the name of the item, such as `Lava`. The 'hits_to_destroy' field indicates the number of hits required to break or destroy the item. In the case of 'Lava', it takes `3` hits to break it. The 'rarity' field denotes the rarity of the item. For `Lava`, it has a rarity of `1`. Finally, the 'grow_time' field specifies the duration, in seconds, required for the item to reach its fully grown state. For `Lava`, it takes `31` ***seconds*** to fully grow.

Type | Name | Description |
:----: |  :----: | ---- |
| number | id | This field stores the id of the item, commonly referred to as itemId (e.g., for the item  `Lava`, the itemId is `4`). |
| string | name | This field stores the name of the item (e.g., `Lava`). |
| number | hits_to_destroy | This field stores the number of hits required to break or destroy the item, whether it's a block or a background (e.g., `Lava` takes `3` hits to break).|
| number | rarity | This field stores the rarity of the item (e.g., `Lava` has a rarity of `1`). |
| number | grow_time | This field stores the time (in ***seconds***) it takes for the item to reach its fully grown state (e.g., `Lava` takes `31` ***seconds*** to fully grow). |

This structure contains functions presented below.
  - None

#### Examples

```lua
local item = item_manager.get_item(2) -- get Dirt item structure
-- item = item structure
print(item.name) -- prints out "Dirt"
```

---


## clothes structure


The clothes structure represents player clothes.

Type | Name | Description |
:----: |  :----: | ---- |
| number | hat | This field stores the itemd_id of hat that the player is wearing |
| number | shirt | This field stores the itemd_id of shirt that the player is wearing |
| number | pants | This field stores the itemd_id of pants that the player is wearing |
| number | shoes | This field stores the itemd_id of shoes that the player is wearing |
| number | face | This field stores the itemd_id of face that the player is wearing |
| number | back | This field stores the itemd_id of back that the player is wearing |
| number | hair | This field stores the itemd_id of hair that the player is wearing |
| number | chest | This field stores the itemd_id of chest that the player is wearing |

This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid") -- get the bot by specified growid (check get_bot() documentation for more info)
local player = bot:get_local_player() -- get player structure
local clothes = player:get_clothes() -- get all clothes that player is wearing
-- clothes = clothes structure

print(clothes.hat) -- prints the hat item_id the player is wearing
print(clothes.shirt) -- prints the shirt item_id the player is wearing
print(clothes.pants) -- prints the pants item_id the player is wearing
print(clothes.shoes) -- prints the shoes item_id the player is wearing
print(clothes.face) -- prints the face item_id the player is wearing
print(clothes.back) -- prints the back item_id the player is wearing
print(clothes.hair) -- prints the hair item_id the player is wearing
print(clothes.hair) -- prints the hair item_id the player is wearing
```

---


## npc structure

The npc structure represents a non-playable character in the game such as bee's, ghost's, pinatas's and etc.

Type | Name | Description |
:----: |  :----: | ---- |
| number | type | This field stores the [npc_type](#npc_type-enum) of the npc |
| number | id | This field stores the unique indentifier of npc |
| [vec2f](#vec2f-structure) | pos | This field stores the position of npc |
| [vec2f](#vec2f-structure) | goal | This field stores the goal position for the npc |
| number | speed | This field stores the speed of npc |



This structure contains functions presented below.
  - None

#### Examples

```lua
local bot = bot_manager.get_bot("growid")
local world = bot:get_world()

for _, npc in pairs(world:get_npcs()) do -- prints all npc's id's in the world
  -- npc = npc structure
  print(npc.id) -- prints out the npc id
end
```

---


# Enums

This section provides documentation on GrowBot enums. Below, you will find tables that represent all the enums available in the GrowBot Lua API.

- Quick links
  - [game_packet_type enum](#game_packet_type-enum) 
  - [npc_type enum](#npc_type-enum)
  - [bot_status enum](#bot_status-enum)

---

## game_packet_type enum

| Number | Name |
| :----: | :--- |
|   0    | state |
|   1    | call_function |
|   2    | update_status |
|   3    | tile_change_request |
|   4    | send_map_data |
|   5    | send_tile_update_data |
|   6    | send_tile_update_data_multiple |
|   7    | tile_activate_request |
|   8    | tile_apply_damage |
|   9    | send_inventory_state |
|   10   | item_activate_request |
|   11   | item_activate_object_request |
|   12   | send_tile_tree_state |
|   13   | modify_item_inventory |
|   14   | item_change_object |
|   15   | send_lock |
|   16   | send_item_database_data |
|   17   | send_particle_effect |
|   18   | set_icon_state |
|   19   | item_effect |
|   20   | set_character_state |
|   21   | ping_reply |
|   22   | ping_request |
|   23   | got_punched |
|   24   | app_check_response |
|   25   | app_integrity_fail |
|   26   | disconnect |
|   27   | battle_join |
|   28   | battle_event |
|   29   | use_door |
|   30   | send_parental |
|   31   | gone_fishin |
|   32   | steam |
|   33   | pet_battle |
|   34   | npc |
|   35   | special |
|   36   | send_particle_effect_v2 |
|   37   | active_arrow_to_item |
|   38   | select_tile_index |
|   39   | send_player_tribute_data |
|   40   | ftue_set_item_to_quick_inventory |
|   41   | pve_npc |
|   42   | pvp_card_battle |
|   43   | pve_apply_player_damage |
|   44   | pve_npc_position_update |
|   45   | set_extra_mods |
|   46   | on_step_on_tile_mod |

#### Examples

```lua

local packet = game_packet:new() -- creates new game_packet
packet.type = game_packet_type.send_lock -- or just packet.type = 15
```

---

## npc_type enum

| Number | Name |
| :----: | :--- |
|   0    | none |
|   1    | ghost |
|   2    | ghost_jar |
|   3    | bee_swarm |
|   4    | harvest_ghost |
|   5    | eye_of_growganoth |
|   6    | ghost_shark |
|   7    | christmas_ghost |
|   8    | blast |
|   9    | pinata |
|   10   | ghost_capture_machine |
|   11   | boss_ghost |
|   12   | mind_control_ghost |
|   13   | ghost_be_gone |
|   14   | hunted_turkey |
|   15   | blaster |
|   16   | thanksgiving_turkey_boss |
|   17   | thanksgiving_turkey_boss_feather_projectile |
|   18   | minion_turkey |

#### Examples

```lua
local type = npc_type.ghost -- type variable will be = 1
print(type) -- prints 1
```

---

## bot_status enum

| Number | Name |
| :----: | :---: |
| 0 | disconnected |
| 1 | connected |
| 2 | connecting |
| 3 | failed_server_data |
| 4 | failed_login |
| 5 | failed_proxy |


#### Examples

```lua
local status = bot_status.connected -- status variable will be = 1
print(status) --  prints 1
```

---
