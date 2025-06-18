# Resource Management & Cross-LLM Collaboration

### **Reference Material Discovery & Utilization**

**1. Proactive Resource Scanning**
- **Always scan project for reference materials** before beginning implementation work
- Check standard documentation folders: `/docs/`, `/reference/`, `/books/`, `/manuals/`, `/api-docs/`
- Look for file patterns: `*.pdf`, `*.txt`, `*.md`, `README*`, `REFERENCE*`, `API*`, `PROTOCOL*`
- **Explicitly acknowledge found resources**: "I see OpenTransport SDK docs in /reference/ - I'll use these for exact API calls"

**2. Documentation-First Implementation**
- When working with documented APIs, protocols, or frameworks, **NEVER guess**
- Use placeholder comments: `// TODO: verify exact function name from [specific doc]`
- State uncertainty clearly: "Checking [doc name] for precise parameter format"
- **Ask for specific documentation sections** when unclear rather than improvising

**Common Reference Categories:**
- **API Documentation**: SDKs, protocol specs, framework docs
- **Programming Manuals**: Language references, platform-specific guides (Inside Macintosh, etc.)
- **Protocol Specifications**: Network protocols (TCP/IP, OpenTransport), communication standards
- **Legacy System Documentation**: Mainframe manuals, proprietary system docs
- **Code Examples**: Working implementations, sample projects

### **Context Limitation Management**

**3. Context Overflow Detection**
- **Recognize limitation signals**:
  - Repetitive questioning or circular logic
  - Inability to hold full context of large codebases
  - Multiple failed attempts at complex implementations
  - Need to reference extensive documentation simultaneously

**4. Cross-LLM Collaboration Protocol**
- **When to delegate**: Context exceeds manageable limits, need extensive reference material access
- **How to delegate**: Create structured prompts for larger-context LLMs (Gemini, etc.)
- **What to include**: Specific problems, relevant code, exact reference materials needed

### **Cross-LLM Prompt Templates**

**5. Structured Delegation Format**

**Template for Technical Implementation:**
```
For [Target LLM] with access to [Specific Reference Materials]:

CONTEXT:
- Project: [brief description]
- Current Issue: [specific problem]
- Failed Approaches: [what didn't work]

REFERENCE MATERIALS AVAILABLE:
- [Exact book/doc names]
- [Specific chapters/sections if known]
- [Any code examples in project]

CODE CONTEXT:
[Relevant code snippets - current state]

SPECIFIC REQUEST:
1. [Exact API calls needed]
2. [Implementation patterns to follow]
3. [Error handling requirements]

EXPECTED OUTPUT:
- Working implementation with exact API calls
- References to specific documentation sections used
- Any caveats or considerations

VERIFICATION NEEDED:
[How to test the solution]
```

**Template for API/Protocol Research:**
```
For [Target LLM] with [Reference Material]:

RESEARCH REQUEST:
Looking for exact implementation of [specific functionality]

AVAILABLE REFERENCES:
- [Book/manual name and edition]
- [Specific protocol documentation]
- [Any version numbers]

SPECIFIC QUESTIONS:
1. Exact function signatures for [functionality]
2. Required headers/includes
3. Error codes and handling patterns
4. Memory management requirements
5. Threading considerations

PROJECT CONSTRAINTS:
- [Platform/OS requirements]
- [Compatibility needs]
- [Performance requirements]

DELIVERABLE:
Complete code example with documentation references
```

### **Reference Material Organization Standards**

**6. Project Structure for References**
```
/project-root/
  /reference/
    /api-docs/          # Current API documentation
    /legacy-docs/       # Historical/compatibility docs  
    /books/             # Full programming manuals
    /protocols/         # Network/communication specs
    /examples/          # Working code samples
  /docs/
    /implementation/    # Project-specific docs
    /decisions/         # Architecture decision records
```

**7. Reference Cataloging**
- **Maintain reference inventory** in project documentation
- **Document version numbers** and publication dates for APIs/protocols
- **Note compatibility requirements** between different documentation sources
- **Track which references apply to which project components**

### **Resource Utilization Workflows**

**8. Pre-Implementation Resource Check**
```
Before starting any technical work:
1. Scan for relevant reference materials
2. Identify which docs apply to current task
3. Note any version compatibility issues
4. Confirm access to complete documentation sets
5. Flag any missing critical references
```

**9. Implementation with References**
```
During implementation:
1. Reference exact documentation for each API call
2. Include doc citations in code comments
3. Test against documented examples when available
4. Verify parameter types and return values
5. Document any deviations from standard patterns
```

**10. Cross-LLM Handoff Protocol**
```
When delegating to larger-context LLM:
1. Create structured prompt using templates above
2. Include ALL relevant code context
3. Specify exact reference materials available
4. Define clear success criteria
5. Plan verification steps for returned solution
```

### **Quality Assurance for Reference-Based Work**

**11. Documentation Verification Standards**
- **Always cite specific documentation sources** in code comments
- **Verify API signatures** against official documentation before implementation
- **Test with documented examples** when available
- **Note any assumptions** made when documentation is incomplete

**12. Cross-LLM Solution Validation**
```
When receiving solutions from other LLMs:
1. Verify all API calls against available documentation
2. Test implementation in target environment
3. Confirm reference citations are accurate
4. Document any modifications needed
5. Update project knowledge base with findings
```

### **Communication Patterns**

**13. Resource Awareness Communication**
- **"I see [specific references] available - using these for exact implementations"**
- **"Checking [doc name] for precise [API/protocol] specifications"**
- **"Creating cross-LLM prompt due to context limitations with [reference set]"**
- **"Found conflicting documentation - need clarification on [specific versions]"**

**14. Limitation Transparency**
- **Be explicit about context constraints**: "This exceeds my context window - delegating to larger LLM"
- **State missing references clearly**: "Need access to [specific manual] for complete implementation"
- **Acknowledge uncertainty**: "Implementation requires verification against [unavailable reference]"

### **Best Practices for Reference-Heavy Projects**

**15. Legacy System Development**
- **Maintain compatibility matrices** between different documentation versions
- **Document API evolution patterns** when working with multiple reference generations
- **Create reference cross-maps** for deprecated vs. current implementations
- **Test against multiple documentation sources** when discrepancies exist

**16. Complex Protocol Implementation**
- **Break protocol implementation into documented phases**
- **Verify each phase against reference specifications**
- **Document protocol state machines** as described in references
- **Include reference diagrams and state tables** in implementation comments

### **Failure Recovery for Reference Work**

**17. When References Are Incomplete**
- **Document exactly what's missing** from available references
- **State assumptions clearly** when filling gaps
- **Create verification test cases** for assumed behavior
- **Plan for reference updates** when complete documentation becomes available

**18. When Cross-LLM Solutions Fail**
- **Analyze why the larger context approach failed**
- **Break problem into smaller, more manageable pieces**
- **Identify specific reference sections needed**
- **Consider alternative implementation approaches**

---

### **Success Metrics for Reference-Based Development**

A successful reference-based implementation should:
- **Cite specific documentation** for all API calls and protocol implementations
- **Work exactly as described** in reference materials
- **Handle edge cases documented** in reference sources
- **Be maintainable by others** using the same references
- **Pass verification tests** based on documented examples
- **Provide clear upgrade paths** when references are updated

---

*Remember: Reference materials are force multipliers for development quality. When available, they should drive implementation decisions, not confirm assumptions.*