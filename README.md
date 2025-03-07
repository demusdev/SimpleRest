# SimpleRest
Sublime Text 4 plugin for sending HTTP requests from any buffer.

Inspired by Emacs rest client.

## Demo
![Screen Recording 2024-07-13 at 23 50 42](https://github.com/user-attachments/assets/df391787-1207-492e-8af4-a5078d193446)

## Request structure
```
Protocol Url
Header_1: Val_1
  ...
Header_n: Val_n
 -- empty line --
Request body
```

Example 1:
```
https://httpbin.org/anything
```

Example 2:
```
GET https://httpbin.org/anything
```

Example 3:
```
GET https://httpbin.org/anything
X-Test-Simplerest: some value
```

Example 4:
```
POST https://httpbin.org/anything
Content-type: application/json

{"x": 5, "y": [6, 7, 8]}
```

## Command
Command for custom key binding is `simplerest_request`:
```
{ "keys": ["super+alt+shift+enter"], "command": "simplerest_request" }
```
