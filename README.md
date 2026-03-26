## WebSocket Server Address Instructions

To connect to the WebSocket server, use the following address:

```
ws://your-websocket-server-address:port
```

### Connection Examples

#### JavaScript
```javascript
const socket = new WebSocket('ws://your-websocket-server-address:port');

socket.onopen = function(event) {
    console.log('Connected to WebSocket server!');
};

socket.onmessage = function(event) {
    console.log('Message from server: ', event.data);
};
```

#### Python
```python
import websocket

ws = websocket.WebSocket()
ws.connect('ws://your-websocket-server-address:port')
print('Connected to WebSocket server!')
ws.send('Hello, Server!')
```
