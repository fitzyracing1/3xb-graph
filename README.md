# 3xb-graph

Interactive D3 force-directed visualization of the 3XB entity graph.
Data is fetched live from the [3XB API](https://3xb-api-production.up.railway.app) `GET /graph` endpoint.

## Usage

Open `index.html` (served via GitHub Pages at https://fitzyracing1.github.io/3xb-graph/).

Query params: `top_n` (default 200, max 1000) and `min_weight` (default 0.5) are passed through to `/graph`;
`api=https://host` points the page at a different API (e.g. `?api=http://localhost:8000`).

The API must send CORS headers (3xb-api currently allows all origins).
