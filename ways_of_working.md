# Ways of Working - Process & Communication Standards

## Enhanced Todo Management & Milestone Tracking

### **Core Todo Principles**
- **Use TodoWrite tool proactively** for all multi-step implementations (3+ steps or complex features)
- Break large features into specific, actionable todo items with clear completion criteria
- Mark only ONE todo as "in_progress" at any time to maintain focus
- **Mark todos as "completed" immediately after finishing each task** - never batch completions
- Present todo status updates to users at logical milestones to maintain transparency

### **Todo Item Quality Standards**

**Good Examples:**
- "Implement user authentication with JWT tokens and bcrypt password hashing"
- "Create PostgreSQL migration for user_sessions table with indexes"
- "Write unit tests for login/logout flow with mock database calls"

**Bad Examples:**
- "Fix authentication" (too vague)
- "Update database" (lacks specificity)
- "Test stuff" (no clear completion criteria)

## Standardized Project Status Documentation

### **Status Documentation Template**
```
### Current Implementation Status

### ✅ Phase 1: [Phase Name] (COMPLETED - 2025-01-07)
- [Specific completed items with verification]
- **Evidence**: [Working code, test results, demo instructions]
- **Verification**: [Step-by-step instructions for user to confirm]

### 🔄 Phase 2: [Phase Name] (IN PROGRESS - Started 2025-01-07)
- [Current todo items with progress indicators]
- **Next Milestone**: [25%/50%/75% checkpoint description]
- **Estimated Completion**: [Realistic timeline]

### 📋 Phase 3: [Phase Name] (PLANNED)
- [Future implementation items]
- **Dependencies**: [What must be completed first]
- **Prerequisites**: [Required decisions or resources]

### Recent Changes
- **2025-01-07**: [Specific change with evidence]
- **2025-01-06**: [Previous change with verification]
```

### **Documentation Standards**
- **Implementation Phase Tracking**: Use visual status indicators (✅ Completed, 🔄 In Progress, 📋 Planned)
- **Recent Changes Log**: Always use current system date (YYYY-MM-DD format) for accurate timestamping
- **Completion Evidence**: Document specific verification steps for each completed phase
- **Progress Transparency**: Regular status updates with concrete evidence

## Milestone Communication Patterns

### **Checkpoint Communication Examples**
- **25% Checkpoint**: "Completed [specific todos]. Architecture validated. [Evidence]. Ready to proceed with [next phase]?"
- **50% Checkpoint**: "Core functionality implemented. [Verification steps]. [Working demo]. Ready for [remaining features]?"
- **75% Checkpoint**: "Feature complete with [concrete evidence]. Testing [specific scenarios]. Ready for final integration?"
- **100% Checkpoint**: "Implementation complete. [Specific evidence]. Verify: [step-by-step instructions]. Confirm before next phase."

## Checkpoint Framework

### **Decision Gates & User Engagement**
- **Phase Start**: Present plan and ask "Ready to proceed with [phase description]?"
- **Mid-Phase**: Show working code/tests and ask for feedback on direction
- **Phase Complete**: Demonstrate functionality and ask "Ready to move to [next phase]?"
- **Architectural Decisions**: Always ask user preference when multiple valid approaches exist

### **Checkpoint Communication Examples**
- **Phase Start**: "Beginning [feature name]. Plan: [specific todos]. Estimated completion: [timeframe]. Ready to proceed?"
- **Mid-Phase**: "Completed [X], currently on [Y]. [Working demo/test results]. Any feedback before continuing?"
- **Phase Complete**: "[Feature] complete. Verify by [specific steps]. Results: [evidence]. Ready for [next phase]?"
- **Architectural Decisions**: "Two approaches for [X]: [Option A - pros/cons] vs [Option B - pros/cons]. Which do you prefer?"

## Evidence Requirements

### **Required Evidence Types**
- **Working Code**: Functional demonstrations, not placeholders
- **Test Results**: Passing tests or clear manual verification steps
- **User Verification**: "Please test [specific feature] and confirm it works as expected"
- **Documentation**: Clear instructions for accessing and verifying each completed feature

### **Evidence-Based Phase Progression**
- Provide concrete evidence before proceeding to next implementation phase (working code, passing tests, screenshots, etc.)
- Include step-by-step verification instructions for each completed phase
- **Stop and communicate** if you cannot provide verifiable evidence of completion
- Ask users to confirm functionality works as expected before continuing
- Document any assumptions or limitations discovered during implementation

## Communication Standards

### **Standard Communication Patterns**
- **Status Updates**: "Completed [X], currently working on [Y], next will be [Z]"
- **Blocking Issues**: "Cannot proceed with [X] because [specific issue]. Suggest [alternatives]"
- **Clarification Requests**: "Two approaches possible for [X]: [Option A] vs [Option B]. Which do you prefer?"
- **Completion Verification**: "Feature [X] is complete. Test by [specific steps]. Ready for next phase?"

### **Implementation Checkpoints & User Engagement**
- **Pause at logical checkpoints** to show concrete progress evidence and ask for user direction
- Use phrases like "Ready to proceed to [next phase]?" before major implementation steps
- **Never assume user intent** - ask specific questions when architectural choices or feature priorities are unclear
- Present working demonstrations or test results before marking phases complete
- Seek user feedback at 25%, 50%, and 75% completion milestones for complex features

---

*These standards ensure consistent, transparent communication and reliable progress tracking throughout project implementation.*