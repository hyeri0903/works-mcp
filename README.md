### ⚒️Setting
~~~
$ mkdir works-mcp
$ cd works-mcp
$ python3 -m venv venv   
$ source venv/bin/activate
$ pip install 'mcp[cli]'  httpx
~~~

### ✅ Setting Cursor, Claude Desktop settings.json
~~~
{
  "mcpServers": {
    "works-mcp": {
      "command": "${Pyhon-Path}",
      "args": ["${main.py file path"],
      "env": {
        "WoRKS_API_TOKEN": "${WORKS_API_TOKEN}"
      }
    }
  }
}

~~~

- python path: $ which python


### ▶️ Run dev mode mcp server
~~~
$ mcp dev main.py
~~~

### ▶️ Run MCP Server Inspector
~~~
$ npx @modelcontextprotocol/inspector dist/index.js
~~~

