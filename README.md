# AI-free-rules

Following are rules for programming sans LLM:

NOTE: LLMs have high utility but I've found that sap my joie de vivre, and
they make you profoundly stupider. 

# Definitions
- AI Agents
  - Sees your code on disk and can automatically make changes.
  - Examples: Claude Code, Codex
  - AI Agents are stronger than AI Chat, so if something is allowed for an AI agent, a fortiori it is allowed for AI Chat.

- AI Chat
  - claude.ai, chatgpt.com, etc.
 
- Library
  - A self contained repository with minimal dependencies that encapsulates a single responsibility.

These following rules are to be followed in an AI free program:

# Rule #1: No AI agent generated code in your project.
- Agents have high timesaving potential to explain existing codebases, generating unit tests etc.
- However, it's too tempting to have it generate code for you. Right now, the agents have you **opting out** of full automation, which makes me very uncomfortable.

# Rule #2: EXCEPTIONS TO RULE #1
- You may use AI agents to write a web frontend
- Rule #7
  
# Rule #3: You may use AI chat to ask high level questions.

# Rule #4: You may use AI chat to read or query API documentation.

# Rule #5: You may use AI chat to fill in well defined functions.

# Rule #6: You may use AI chat to write build system code (makefiles, CMake, etc.)
- This carries some risk and may be changed in the future.

# Rule #7: You can use AI chat or AI agents to write a library, with caveats
- Caveat #1: The library needs to be its own distinct repository with minimal dependecies (i.e. it can't import from the main project)

# Rule #8: You may use AI chat to code review and suggest changes to your code
- This must be done with care, as enough context needs to be provided
