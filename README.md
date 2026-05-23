# AI-free-rules

Following are rules for programming sans LLM:

NOTE: LLMs have high utility but I've found that sap my joie de vivre, and
they make you profoundly stupider. 

# Definitions
- AI Chat
  - Examples: claude.ai, chatgpt.com
  - Lets you type a prompt and/or paste text/upload artifacts.
  - Burns low number of tokens (unless in thinking mode) and can be in free tier.
  - Doesn't necessarily have context for your project.
    
- AI Agents
  - Examples: Claude Code, Codex
  - Sees your code on disk. Thus, has full context of your project.
  - Burns high number of tokens.
  - Can run autonomously. Usually an *opt-out* of automatic changes, which makes me uncomfortable.
  - AI Agents are stronger than AI Chat, so if something is allowed for an AI agent, is allowed _a fortiori_ for AI Chat.

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
