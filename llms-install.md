# MDataAccess MCP installation

MDataAccess is a hosted remote MCP server. No local package, Docker image, API key, or build step is required to connect the MCP server.

## Endpoint

- Transport: Streamable HTTP
- URL: https://api.mdataaccess.com/mcp/

## MCP configuration

Add MDataAccess as a remote HTTP MCP server using:

```json
{
  "mcpServers": {
    "mdataaccess": {
      "url": "https://api.mdataaccess.com/mcp/"
    }
  }
}
```

After connecting, the client should discover these seven tools:

- read_webpage
- enrich_company
- enrich_person
- search_people
- search_companies
- find_decision_maker
- find_lead

MDataAccess uses x402 pay-per-request access for protected API operations. Connecting to the MCP server and discovering tools does not itself purchase data.

Website: https://mdataaccess.com
