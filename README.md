# qbo-connect

Public pages required by Intuit for the private **Claude Bookkeeping Agent MCP** app of GOSS Auto Parts Ltd.:

| Page | Intuit field |
|---|---|
| `index.html` | Launch URL, Connect/Reconnect URL |
| `disconnect.html` | Disconnect URL |
| `privacy.html` | Privacy policy URL |
| `eula.html` | End-user licence agreement URL |
| `callback.html` | Production OAuth redirect URI |

`callback.html` forwards QuickBooks' one-time sign-in code to the sign-in helper on the local computer (`http://localhost:8000/callback`). It stores and sends nothing else. The code is useless without the app's client secret, which is never published.

The MCP server itself and all QuickBooks data stay on the company computer.
