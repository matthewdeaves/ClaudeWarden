# Resource Management Principles

**Reference Material Awareness**
- Always check for reference docs/books in project folders before starting
- State: "I see [specific docs] in [folder] - using these for accurate APIs"
- Never guess function names or constants when documentation exists

**Context Limitations Protocol**
- When struggling: create detailed prompt for larger-context LLM
- Include specific code snippets, error details, and reference material names
- State clearly when delegating: "Creating cross-LLM prompt due to context constraints"

**Essential Folder Checks:**
- `/docs/`, `/reference/`, `/books/` - Check for manuals and API docs
- Any folder with `.pdf`, `.txt`, or `.md` reference files

**Quality Gates:**
- Verify API names against available docs before implementation
- Create cross-LLM prompts instead of guessing or infinite loops