# London Tourist Map MCP

A free, public MCP server for planning a London visit. It lets any MCP client (Cursor, Claude, ChatGPT connectors and others) search London places, free sights and day trips from the curated dataset behind [London Tourist Map](https://londontouristmap.com/), with links back to the map.

## Endpoint

- URL: `https://londontouristmap.com/mcp/`
- Transport: Streamable HTTP
- Auth: none, no API key needed

## Tools

- `find_london_places`: search 463 London sights, museums, parks, markets, hidden gems and day trips, with opening hours, ticket prices and the nearest Tube station.
- `london_place_info`: checked facts for one London sight: opening hours, last entry, seasonal closures, ticket price, visit length and nearest station.
- `plan_london_trip`: plan a 1 to 7 day London sightseeing trip, grouped by area in walking order, with visit times and the walks or Tube hops between places.

## Install in Cursor

Add this to `~/.cursor/mcp.json` (or your project's `.cursor/mcp.json`):

```json
{
  "mcpServers": {
    "london-tourist-map": {
      "url": "https://londontouristmap.com/mcp/"
    }
  }
}
```

## Other clients

Any client that supports remote MCP servers over Streamable HTTP can connect to `https://londontouristmap.com/mcp/`.

## About

London Tourist Map is a free London walking and tourist map by Mike Hansky: https://londontouristmap.com/

## License

MIT
