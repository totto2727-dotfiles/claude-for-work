# Search External Documentation

This command efficiently searches external documentation with optimized tool selection to minimize execution time.

$ARGUMENTS

## Optimized Search Strategy

Query: "$ARGUMENTS"

### Primary Search (Choose ONE)

**Option A: Effect Documentation** (if query contains: Effect, pipe, function composition, functional programming, Effect-TS)
- Use totto-doc-mcp search_ai_effect tool ONLY
- Provide comprehensive results from Effect ecosystem

**Option B: Library Documentation** (for all other queries)
- Use context7 resolve-library-id + get-library-docs
- Get detailed documentation with high token limit (8000-10000)
- No topic restriction - retrieve comprehensive documentation

### Fallback Only When Necessary

**Option C: Web Search** (ONLY if Options A/B fail completely)
- Use /user:gemini-search slash command
- Provide targeted search with "$ARGUMENTS" query
- High-speed alternative to MCP tools

## Efficiency Rules

1. **Single Tool Focus**: Use the most appropriate tool based on query analysis
2. **High Token Limits**: Request comprehensive documentation in one call
3. **No Deep Exploration**: Avoid follow-up searches unless critical information is missing
4. **Fast Failure**: If primary tool fails, briefly try fallback, then conclude

## Success Criteria

- Complete search in 1-2 tool calls maximum
- Provide sufficient information to answer the user's question

Execute optimized search for: "$ARGUMENTS"
