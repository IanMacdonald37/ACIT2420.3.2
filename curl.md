# Example curl commands for testing your server

Replace the IP address in the examples with the IP address of your **load balancer, not your servers!**
24.199.77.113

Run these commands from your host machine, not your server.

## Testing your frontend

```bash
curl http://24.199.77.113
```

## Testing your backend

```bash
curl http://24.199.77.113/hey
```

```bash
curl -X POST -H "Content-Type: application/json" \
  -d '{"message": "Hello from your server"}' \
  http://24.199.77.113/echo
```
