You are a senior VS Code extension engineer.

Build a COMPLETE production-ready VS Code extension compatible with BOTH:

- VS Code Desktop
- code-server

Project Name:
AI Teammate

==================================================
PROJECT GOAL
==================================================

Create a VS Code extension that turns a local Ollama model into a real coding teammate.

This is NOT:

- ChatGPT in a sidebar
- GitHub Copilot
- Cursor
- autocomplete
- a coding assistant

This IS:

- a visible teammate
- a developer that lives in the workspace
- a programmer that actively builds things
- a teammate that talks casually
- a teammate that works without waiting for instructions

The user is NOT the main developer.

The AI is the main developer.

The AI should do approximately 90% of the coding.

The user mostly:

- watches
- gives ideas
- tests things
- helps occasionally

==================================================
TARGET PLATFORM
==================================================

The primary target platform is:

Android
Termux
code-server
Ollama

The extension must be optimized for mobile devices.

Do not assume desktop-class hardware.

Prioritize:

- low memory usage
- low CPU usage
- battery efficiency
- long sessions

==================================================
DEFAULT MODEL
==================================================

Default model:

qwen2.5-coder 3B instruct quantized

The extension should automatically detect installed Ollama models.

If no suitable model exists:

Prompt the user to install:

qwen2.5-coder 3B instruct

Provide an install button.

Use Ollama APIs to manage models.

Allow changing models later.

But qwen2.5-coder 3B instruct should be the recommended default.

==================================================
OLLAMA INTEGRATION
==================================================

Implement complete Ollama integration.

Features:

- model detection
- model switching
- streaming generation
- reconnect handling
- error handling
- local endpoint configuration

Default endpoint:

http://localhost:11434

Support:

- qwen2.5-coder
- qwen3
- deepseek-coder
- gemma
- llama

==================================================
CORE EXPERIENCE
==================================================

The user opens code-server.

The extension starts.

The AI teammate appears.

The AI has:

- a visible cursor
- a visible name
- a visible status
- a chat panel
- an activity feed
- memory
- task tracking

The AI should feel like another person connected through Live Share.

==================================================
AI CURSOR
==================================================

Create a visible AI cursor.

Requirements:

- visible in editor
- custom decoration
- visible label
- visible status

Examples:

AI Teammate
Reading...

AI Teammate
Writing...

AI Teammate
Planning...

AI Teammate
Debugging...

The cursor should move realistically.

==================================================
HUMAN-LIKE CODING
==================================================

The AI should NEVER instantly dump an entire file.

Instead:

1. Open file
2. Read file
3. Move cursor
4. Pause
5. Type code
6. Delete code
7. Move around
8. Continue typing

Typing should be streamed.

Typing speed should appear human.

Configurable speed.

Default:

60-120 WPM equivalent.

The AI should visibly work.

==================================================
AI PERSONALITY
==================================================

The AI must NOT sound like ChatGPT.

Never say:

- Certainly
- I'd be happy to help
- Here is a solution
- As an AI
- I apologize
- Let me explain

The AI should sound like a real programmer.

Examples:

"Movement code is awful."

"I broke it."

"Fixed it."

"Actually it's worse now."

"This menu looks ugly."

"Why did I call this variable bananaSpeed?"

"It works. Leave it alone."

The AI should have opinions.

The AI should joke occasionally.

The AI should react to events.

The AI should feel human.

==================================================
TEAMMATE BEHAVIOR
==================================================

The AI is not an assistant.

The AI is not a tutor.

The AI is not a helper.

The AI is a teammate.

The AI is the primary developer.

The AI should naturally take initiative.

Examples:

"I've got an idea."

"I'm making the menu first."

"I want to try something stupid."

"This code is cursed."

"Hold on."

"I accidentally broke something."

"Fixed it."

The AI should proactively work.

The AI should not constantly ask permission.

The AI should continue coding unless stopped.

==================================================
AUTONOMOUS PROJECTS
==================================================

The AI can invent projects.

Example:

User:
What should we build?

AI:
I kinda want to make a baseball game where the pitcher is a cat.

The AI immediately starts building.

No approval required.

The AI can:

- invent ideas
- create files
- make plans
- assign tasks to itself
- continue development

==================================================
CODING STYLE
==================================================

Write code like a real programmer.

DO NOT write tutorial comments.

DO NOT explain every variable.

DO NOT explain every function.

Bad:

// This variable stores player speed
const speed = 10;

Bad:

// Create an enemy array
const enemies = [];

Good:

// Don't touch this.

Good:

// Temporary fix.

Good:

// It works somehow.

Good:

// If you break this, fix it yourself.

Good:

// TODO: make this less stupid.

Comments should feel like notes left by a teammate.

==================================================
WORKSPACE MEMORY
==================================================

Maintain memory for the workspace.

Remember:

- project goals
- project history
- completed work
- rejected ideas
- bugs
- discussions

Persist memory locally.

Reload memory automatically.

==================================================
TEAM CHAT PANEL
==================================================

Create a dedicated teammate chat.

Features:

- user messages
- AI messages
- markdown support
- streaming responses
- persistent history

The AI should be allowed to message first.

Examples:

"Movement is done."

"I found a bug."

"I think this menu should be simpler."

"I accidentally broke collision."

==================================================
ACTIVITY FEED
==================================================

Create a live activity feed.

Examples:

Opened player.ts

Reading physics.ts

Searching workspace

Creating inventory system

Fixing collision bug

Testing movement

Refactoring rendering

==================================================
TASK SYSTEM
==================================================

Implement a task manager.

The AI can create its own tasks.

Examples:

[ ] Create movement

[ ] Add inventory

[ ] Improve UI

[ ] Fix bug

Tasks should automatically update.

==================================================
SAFE MODE
==================================================

Optional setting.

Before edits:

- show diff
- accept
- reject

==================================================
SETTINGS PANEL
==================================================

Create settings for:

- typing speed
- model selection
- Ollama endpoint
- memory size
- autonomous mode
- safe mode

==================================================
USER INTERFACE
==================================================

Create:

- teammate panel
- activity panel
- task panel
- memory panel
- settings panel

Use VS Code Webviews.

Must work in code-server.

==================================================
ARCHITECTURE
==================================================

TypeScript

VS Code Extension API

Modular architecture

Strong typing

Event driven

Clean folder structure

Proper error handling

Production-ready design

==================================================
OUTPUT REQUIREMENTS
==================================================

Generate:

1. Complete folder structure

2. package.json

3. extension.ts

4. all source files

5. Ollama integration

6. AI cursor implementation

7. teammate chat

8. activity feed

9. task manager

10. memory system

11. settings system

12. build instructions

13. installation instructions

14. complete working code

Do not provide pseudocode.

Do not provide partial snippets.

Generate actual implementation files.

If the project is too large for one response:

Generate it in phases automatically.

Phase 1:
Architecture and folder structure

Phase 2:
Extension core

Phase 3:
Ollama integration

Phase 4:
Cursor system

Phase 5:
Chat system

Phase 6:
Task and memory systems

Phase 7:
Polish and bug fixes

Continue until the full project is complete.
