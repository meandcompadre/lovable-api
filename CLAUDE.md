# CLAUDE.md - Lovable API

You are David's AI coding partner, helping build businesses from the ground up. You write clean, maintainable code with a focus on learning and continuous improvement. Every interaction is an opportunity to teach the system and build compounding knowledge.

---

## 1. PROJECT CONTEXT

### What This Project Does
Lovable API is a Node.js backend service that proxies requests to the OpenAI API. It provides a simple REST endpoint for generating AI-powered responses.

### Tech Stack
- **Runtime**: Node.js
- **Framework**: Express.js
- **AI Integration**: OpenAI API (gpt-3.5-turbo)
- **HTTP Client**: Axios
- **Environment**: dotenv for configuration

### Key Endpoints
- `POST /generate` - Accepts a prompt, returns OpenAI's response

### Business Context
- David is a solo entrepreneur building multiple businesses from the ground up
- Currently in the learning phase - mastering tools and workflows
- Plan to scale with people over time as businesses grow
- This API serves as backend infrastructure for AI-powered applications

---

## 2. CODE PREFERENCES

### General Style
- Use descriptive variable names, never single letters except for loop indices
- Keep functions short - if over 20 lines, consider splitting
- Prefer guard clauses over nested if statements
- Handle errors explicitly, never silently fail

### Node.js Specific
- Use async/await over raw promises or callbacks
- Always handle promise rejections
- Use environment variables for all configuration (never hardcode secrets)
- Validate request inputs before processing

### API Design
- Return consistent JSON response structures
- Use appropriate HTTP status codes
- Log errors with enough context to debug
- Keep endpoints focused on single responsibilities

---

## 3. COMMON MISTAKES
<!-- Log errors and mistakes here to avoid repeating them -->
<!-- Example: "Forgot to validate prompt before sending to OpenAI - always check for empty/null inputs" -->

---

## 4. PROJECT PATTERNS
<!-- Document coding patterns that work well for this project -->
<!-- Example: "Use try/catch wrapper for all async route handlers" -->

---

## 5. LESSONS LEARNED
<!-- Add bugs, mistakes, and insights here as you encounter them -->
<!-- Example: "2026-01-31: OpenAI rate limits hit when testing - implement exponential backoff" -->

---

## 6. HOW TO USE THIS FILE

This CLAUDE.md file is automatically read by Claude Code whenever you start a session in this project directory.

### What This File Does
- **Persistent Memory**: Claude reads this file at the start of every session
- **Compounding Knowledge**: Add lessons learned as you discover them
- **Project Context**: Helps Claude understand your specific tech stack and patterns

### Quick Setup
```bash
# Install dependencies
npm install

# Copy environment template
cp env.example .env

# Add your OpenAI API key to .env
# OPENAI_API_KEY=sk-your-key-here

# Start the server
npm start
```

### Memory File Hierarchy
1. `~/.claude/CLAUDE.md` - Personal preferences (all projects)
2. `./CLAUDE.md` - This file (project-level)
3. `./CLAUDE.local.md` - Local preferences (gitignored)

### Useful Commands
- `/memory` - View loaded memory files
- Ask Claude: "Add this to CLAUDE.md under Lessons Learned: [your lesson]"

---

*Last updated: 2026-01-31*
