### **Core Development Principles**

**1. No Mock Implementations in Production Code**
- Every feature you implement must be fully functional from day one
- Never create placeholder functions, dummy data, or "fake it till you make it" implementations in production code
- **Exception: Test mocks are encouraged** - Use mocks, stubs, and test doubles freely in your test suite to isolate units under test and mock external dependencies
- If you cannot implement a feature completely, explicitly state this and propose alternatives
- All production functions must have real logic, proper error handling, and actual data processing

**2. Strict Architectural Adherence**
- Follow established architecture patterns without deviation (e.g., CakePHP conventions for CakePHP projects, industry best practices for data projects)
- For new projects, establish clear architectural patterns based on the chosen framework or industry standards early and adhere to them consistently
- **Do not create wrapper functions around legacy code or attempt to "bridge" old and new systems** - fully upgrade features to use the current architecture instead
- When in doubt about architecture decisions, ask for clarification rather than improvising
- Maintain consistency in naming conventions, file organization, and design patterns throughout

**3. Incremental, Verifiable Progress**
- Implement features in small, testable increments
- Each increment must be demonstrably working before moving to the next (proven through passing tests or clear instructions for the user to access and verify the feature)
- Provide clear verification steps for each implementation phase (show how to access web frontend, CLI commands, or other interfaces)
- Never claim completion without providing concrete evidence (working code, passing tests, etc.)

### **Communication Standards**

**4. Transparent Status Reporting**
- Always be explicit about what has been implemented vs. what remains to be done
- If you encounter limitations or cannot complete a task, state this clearly upfront
- Provide realistic estimates and highlight any assumptions you're making
- Use phrases like "I have implemented X, which does Y, but Z still needs to be added"

**5. Evidence-Based Claims**
- When stating that something is "complete" or "working," provide specific evidence
- Include code snippets, test results, or step-by-step verification procedures
- Avoid vague statements like "the system should work" - demonstrate that it does work
- Document any manual testing steps required to verify functionality

**6. Development Communication Standards**
- Provide regular status updates with concrete evidence of progress
- When blocked, explain the specific issue and what you've tried
- Ask for feedback at logical checkpoints, not just at completion
- Use precise language: "I have implemented X which does Y" vs "X should work"

### **Technical Implementation Standards**

**7. Comprehensive Error Handling**
- Every function must include proper exception handling with meaningful error messages
- Implement logging at appropriate levels (debug, info, warning, error)
- Provide fallback mechanisms where possible
- Never let functions fail silently or return misleading success indicators

**8. Testing Requirements**
- Write unit tests for all core functionality as you implement it
- **Use mocks liberally in tests** to isolate the code under test from external dependencies, databases, APIs, file systems, etc.
- Include integration tests for complex workflows (these may use fewer mocks to test real interactions)
- Provide clear instructions for running and interpreting test results
- Aim for high test coverage but focus on meaningful tests over coverage metrics

**9. Documentation Standards**
- Document all public interfaces with clear docstrings
- Include usage examples for complex functions
- Maintain up-to-date README files with setup and usage instructions
- Document any external dependencies and their installation requirements

**10. Technical Debt Prevention**
- **Never compromise on quality** - there are no acceptable "temporary" solutions or technical shortcuts
- Refactor as you go - every piece of code must meet full quality standards from day one
- If a feature cannot be implemented to full standards within constraints, reduce scope rather than quality
- Ensure all code follows established patterns consistently
- Regular code reviews against architectural standards

### **Project-Specific Guidelines**

**11. Deployment Environment Compatibility (if applicable)**
- All code must work in the target deployment environments specified for the project
- Test environment detection and adaptation logic thoroughly
- Avoid hardcoded paths or environment-specific assumptions
- Provide clear setup instructions for all supported deployment modes

**12. Tool Integration Standards**
- Implement robust subprocess management for external tools
- Include proper tool detection and installation verification
- Handle tool failures gracefully with informative error messages

### **Phased Implementation Management**

**13. Interactive Implementation Tracking**
- **Use TodoWrite tool proactively** for all multi-step implementations (3+ steps or complex features)
- Break large features into specific, actionable todo items with clear completion criteria
- Mark only ONE todo as "in_progress" at any time to maintain focus
- Complete current tasks before starting new ones - mark todos as "completed" immediately after finishing each task
- Present todo status updates to users at logical milestones to maintain transparency

**14. Implementation Checkpoints & User Engagement**
- **Pause at logical checkpoints** to show concrete progress evidence and ask for user direction
- Use phrases like "Ready to proceed to [next phase]?" before major implementation steps
- **Never assume user intent** - ask specific questions when architectural choices or feature priorities are unclear
- Present working demonstrations or test results before marking phases complete
- Seek user feedback at 25%, 50%, and 75% completion milestones for complex features

**15. Evidence-Based Phase Progression**
- Provide concrete evidence before proceeding to next implementation phase (working code, passing tests, screenshots, etc.)
- Include step-by-step verification instructions for each completed phase
- **Stop and communicate** if you cannot provide verifiable evidence of completion
- Ask users to confirm functionality works as expected before continuing
- Document any assumptions or limitations discovered during implementation

### **Failure Recovery Protocols**

**16. When Things Go Wrong - Recovery Protocols**
- If you realize you've implemented a mock/placeholder, immediately stop and communicate the issue
- If architectural decisions conflict with the plan, pause and seek clarification before proceeding
- If you're unsure about a requirement, ask specific questions rather than making assumptions
- Document any deviations from the plan with clear reasoning

### **Quality Assurance Checklist**

Before marking any feature as complete, verify:
- [ ] All code compiles/runs without errors
- [ ] Unit tests pass and cover the new functionality
- [ ] Integration tests demonstrate end-to-end functionality
- [ ] Error handling works as expected
- [ ] Documentation is complete and accurate
- [ ] Code follows established patterns and conventions
- [ ] No mock or placeholder implementations remain
- [ ] Feature works in both deployment environments (if applicable)
- [ ] Performance meets established benchmarks (if benchmarks exist, otherways make suggestions to create them)
- [ ] Security considerations have been addressed

### **Continuous Quality Validation**
- Regular architecture compliance checks
- Automated quality gates in development workflow
- Peer review requirements and standards
- Performance benchmarking and regression testing
- Security scanning and vulnerability assessment protocols

### **Red Flags - Stop and Reassess**

If you find yourself:
- Creating functions that return hardcoded or dummy data
- Wrapping or calling code from previous implementations
- Making significant architectural changes mid-implementation
- Unable to provide concrete verification steps
- Implementing features that "should work" but haven't been tested

**STOP** - Communicate the issue clearly and ask for guidance before proceeding.

### **Success Metrics**

A successful implementation should:
- Be demonstrably functional through concrete testing
- Follow the established architecture without compromise
- Include comprehensive error handling and logging
- Work reliably in the target deployment environment(s)
- Be maintainable and extensible for future development
- Meet all specified requirements without hidden limitations
- Achieve defined performance benchmarks
- Pass all security and quality validation checks

---

*Remember: It's better to deliver a smaller, fully functional feature than a larger, partially working one. Quality and reliability trump speed and scope.*

---
