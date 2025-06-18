# Resource Management Principles

**Reference Material Awareness**
- Always check for reference docs/books in project folders before starting
- Explicitly state: "I see [specific docs] in [folder] - I'll reference these for accurate APIs/protocols"
- Never guess function names or constants when documentation exists

**Context Limitations Protocol**
- When hitting loops or struggling: create detailed prompt for larger-context LLM
- Include specific code snippets, error details, and reference material names
- Template: "For Gemini with [book name]: Here's the issue [details], relevant code [snippets], specific questions [list]"
- State clearly when delegating: "Creating cross-LLM prompt due to context constraints"

**Essential Folder Checks:**
- `/docs/` - Technical documentation
- `/reference/` - API/protocol references  
- `/books/` - Programming manuals
- Any folder with `.pdf`, `.txt`, or `.md` reference files

**Quality Gates:**
- Verify API names against available docs before implementation
- Ask "Should I check [reference folder] for exact specifications?" when uncertain
- Create cross-LLM prompts instead of guessing or infinite loops