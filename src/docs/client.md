# client table

## Functions

## **load_script(scriptname)**

Type | Name | Description
------------ | ------------- | ------------
string | scriptname | Script name

Load the script
```lua
client.load_script("example.lua")
```

---

## **unload_script(scriptname)**

Type | Name | Description
------------ | ------------- | ------------
string | scriptname | Script name

Unload the script
```lua
client.unload_script("example.lua")
```

---

## **register_callback(eventname, fn)**
Type | Name | Description
------------ | ------------- | ------------
string | eventname | Callback name
function | fn | Lua function()

---

## **get_username()**: string

Returns your cheat username
```lua
local username = client.get_username()
```
---

## **notify(text)**
Type | Name | Description
------------ | ------------- | ------------
string | text | Notification text

Pushing notification
```lua
client.notify("Hello world!")
```
---

## **get_time_stamp()**: number

Returns the unix timestamp
```lua
local timestamp = client.get_time_stamp()
```
---

## **get_system_time()**: number, number, number

Returns the windows time
```lua
local hours, minutes, seconds = client.get_system_time()
```
---

## **is_key_pressed(key)**: bool
Type | Name | Description
------------ | ------------- | ------------
number | key | Virtual key code

Returns true if key pressed
```lua
local pressed = client.is_key_pressed(1)
```
---

## **is_key_clicked(key)**: bool
Type | Name | Description
------------ | ------------- | ------------
number | key | Virtual key code

Returns true if key clicked
```lua
local clicked = client.is_key_clicked(1)
```
---

## **find_pattern(module, pattern)**: number
Type | Name | Description
------------ | ------------- | ------------
string | module | Module
string | pattern | Pattern

Returns pattern address
```lua
local line_goes_through_smoke_addr = client.find_pattern("client_panorama.dll", "55 8B EC 83 EC 08 8B 15 ? ? ? ? 0F 57 C0")
```
---