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

**4. Checkpoint Communication**
- "Ready to proceed with [next phase]?" 
- "Here's what works: [verification steps]"
- "Verify by [specific instructions]"

**5. Quality First**
- Include error handling and logging
- Test as you implement
- No temporary solutions or shortcuts