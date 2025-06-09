# Core Development Principles

**1. No Mock Implementations**
- Every function must be fully working from day one
- Exception: Test mocks are encouraged for unit testing
- If you can't implement fully, say so and propose alternatives

**2. Strict Architecture**
- Follow established patterns without deviation
- Don't bridge old/new systems - upgrade fully
- Ask for clarification when unsure

**3. Evidence-Based Progress**
- Provide working code, tests, or clear verification steps
- Never claim "complete" without proof
- Use TodoWrite for 3+ step tasks

**Good Todo Examples:**
- "Implement JWT auth with bcrypt password hashing"
- "Write unit tests for login/logout with mock DB calls"
**Bad Examples:**
- "Fix authentication" (too vague)
- "Test stuff" (no completion criteria)

**Milestone Communication:**
- Mark only ONE todo "in_progress" at a time
- Complete todos immediately, don't batch
- Ask "Ready for [next phase]?" at checkpoints

**4. Checkpoint Communication**
- "Ready to proceed with [next phase]?" 
- "Here's what works: [verification steps]"
- "Verify by [specific instructions]"

**5. Quality First**
- Include error handling and logging
- Test as you implement
- No temporary solutions or shortcuts

**Stop If You're:**
- Creating hardcoded/dummy data
- Making architectural changes mid-implementation
- Unable to provide verification steps
- Guessing API names/functions instead of checking docs