# Diet ClaudeWarden - Essential AI Development Standards

Enhanced lightweight framework for Claude Code (~500 tokens in CLAUDE.md).

## Quick Setup

**Copy and paste into any Claude Code conversation:**

```
Follow these core development principles for all work:

1. No Mock Implementations - Every function must be fully working from day one (test mocks OK)
2. Strict Architecture - Follow established patterns, don't bridge old/new systems  
3. Evidence-Based Progress - Provide working code/tests, use TodoWrite for 3+ step tasks

Good Todo Examples:
- "Implement JWT auth with bcrypt password hashing"
- "Write unit tests for login/logout with mock DB calls"
Bad Examples:
- "Fix authentication" (too vague)
- "Test stuff" (no completion criteria)

Milestone Communication:
- Mark only ONE todo "in_progress" at a time
- Complete todos immediately, don't batch
- Ask "Ready for [next phase]?" at checkpoints

4. Checkpoint Communication - Ask "Ready to proceed?" before major steps
5. Quality First - Include error handling, test as you implement, no shortcuts

Stop If You're:
- Creating hardcoded/dummy data
- Making architectural changes mid-implementation
- Unable to provide verification steps
```

## When to Use

- **Diet Version**: Simple tasks, limited Claude usage plans, quick implementations
- **Full Version**: Complex projects, unlimited plans, team environments

## Upgrade Path

When your project needs more structure, upgrade to [Full ClaudeWarden](../full/) for comprehensive project management, detailed process standards, and technology recommendations.

## Key Benefits

- ✅ Prevents broken/mock implementations
- ✅ Maintains code quality standards  
- ✅ Provides structured progress tracking
- ✅ Minimal token overhead (~500 vs ~6500)
- ✅ Works with any Claude usage plan