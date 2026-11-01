# Uganda Land Parcels & Kampala Block/Plot Lookup MCP

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Kampala land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- The Ministry of Lands' 2024 cadastre for Kampala and the edge of Wakiso, as KCCA publishes it
- Parcel lookup by cadastral number (`KCCA-71_1_22_NW_3-90941`), block and plot (`Block 9 Plot 123`), a whole block (paged), or coordinates
- Registration status and history (current, pending, previous, historic), surveyed area, land use, road, county and division
- Satellite and street map images of a parcel and its neighbours, labelled by plot number

Greater Kampala only. Parcels have no owner or title information.

## Connect

```
https://bumiatlas.com/mcp/uganda
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/uganda](https://bumiatlas.com/mcp-docs/uganda).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `UG_parcel_search` | Find parcels by cadastral number, block and plot, a whole block (paged), or `latitude, longitude`; each result is the whole record, the boundary as GeoJSON on request |
| `UG_parcel_image` | Satellite or street map image of a parcel or point, with every current and pending parcel in view outlined and labelled with its plot number |

## Example prompts

- *"Which parcel is at 0.28217, 32.55893?"*
- *"Look up Block 11 Plot 915 and its registration history."*
- *"Find cadastral number KCCA-71_1_22_NW_3-41430 and show it on satellite imagery."*
- *"What is the surveyed area of this plot?"*

## Data source

Cadastre © Ministry of Lands, Housing and Urban Development (MLHUD), Uganda, Cadaster 2024 as published by KCCA. A copy of public data for research, not a legal land record.
