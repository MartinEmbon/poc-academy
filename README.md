# Digibee Academy Explorer

CSM tool to query student progress in Digibee Academy via MCP (Model Context Protocol).

## Tools Available

- **search_student** — Search by student name or email
- **search_by_company** — Search all students from a company

## Setup

```bash
npm install
npm start
```

Open `http://localhost:3001`

## Environment Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `PORT` | `3001` | Server port |
| `MCP_ENDPOINT` | `https://test.godigibee.io/pipeline/digibee/v1/mcp-server-digibee-academy/mcp` | MCP server URL |

## Deploy on Render

1. Push to GitHub
2. Create a new **Web Service** on Render
3. Set **Build Command**: (leave empty, no build needed)
4. Set **Start Command**: `node server.js`
5. Optionally set `MCP_ENDPOINT` env var if different from default

## Project Structure

```
├── server.js          # Node.js server + MCP client
├── package.json
├── public/
│   ├── index.html     # Chat UI
│   └── logo.png       # Digibee Academy logo
└── README.md
```
