
# Node network

Automated bot for NodeNetworkGo platform with support for multiple accounts and proxy configurations (HTTP/SOCKS).


#Register
Register https://node.optimai.network/register?ref=0DE4A506


## Features

- Multi-account support
- HTTP and SOCKS proxy support
- Automatic periodic pinging
- Detailed logging with colored output
- Account status monitoring
- Graceful shutdown handling

## Prerequisites

- NodeNetwork.js (v16 or higher)
- npm (NodeNetwork Package Manager)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/andywp/NodeNetwork_network.git
cd NodeNetworkGo-Auto-Bot
```

2. Install dependencies:
```bash
npm install
```
## Configuration

1. Create `data.txt` in the project root:
   - Add one NodeNetworkGo token per line
   - Example:
     ```
     token1
     token2
     token3
     ```

2. (Optional) Create `proxies.txt` in the project root:
   - Add one proxy per line
   - Supports both HTTP and SOCKS proxies
   - Example:
     ```
     http://ip1:port1
     socks5://ip2:port2
     socks4://ip3:port3
     ```

## Usage

Run the bot:
```bash
node index.js
```



## Troubleshooting

Common issues and solutions:

1. Proxy Connection Errors:
   - Verify proxy format is correct
   - Check if proxy is online and accessible
   - Ensure proxy supports HTTPS connections

2. Authentication Errors:
   - Verify token is valid and not expired
   - Check if token has proper permissions

3. Rate Limiting:
   - The bot automatically handles rate limiting with 3-second delays between pings
   - If you encounter rate limits, consider increasing the delay

## Contributing

Feel free to fork the repository and submit pull requests for any improvements.

## License

