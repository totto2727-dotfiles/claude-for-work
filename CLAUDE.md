# Claude Code Guidelines

## Basic Rules

- **Parallel Execution**: Execute independent processes concurrently
- **Information Gathering**: Use Context7 MCP for library information
- **Planning**: Always create and confirm execution plans unless instructed otherwise

## Language Rules

- **Chat Response**: Always respond in Japanese
- **Markdown Output**: Always output documentation in Japanese
- **Commit Messages**: Follow the language pattern of existing commits in the repository

## Development Rules

- Avoid hardcoding values
- Follow existing code patterns
- Manage sensitive information properly
- Strictly follow Conventional Commits

### Code Analysis and Search

- **serena MCP Priority**: When serena MCP is available, use serena MCP tools for code search and analysis
- **Claude Code Output**: Always use Claude Code's built-in functionality for code output and file modifications
  - serena MCP diffs are difficult to read; Claude Code provides clearer change visualization
