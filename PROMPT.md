# Original Prompt Used to Generate This Repository

Below is the exact prompt used to bootstrap this AI engineering workflow architecture:

---

You are an expert in GitHub Copilot, AI agentic systems, and developer workflow design.
I want you to DESIGN and GENERATE a complete reusable AI engineering workflow system for GitHub Copilot that is:
- Instruction-driven (NOT prompt-heavy)
- Token-efficient
- Adaptive (simple vs complex tasks)
- Scalable across teams
- Based on real developer workflows (e.g., JIRA tickets)
- Documented as a reusable pattern
- Accompanied by clear visual diagrams
---
# 🎯 OBJECTIVE
Create a production-ready Copilot workflow system where:
- Developers paste requirements (e.g., JIRA tickets) into Copilot chat
- The system automatically:
  - Understands intent
  - Detects complexity
  - Validates requirement quality (when needed)
  - Routes execution intelligently
  - Executes using implicit modes (no explicit agent calls)
---
# 🔷 CORE ARCHITECTURE
## ✅ copilot-instructions.md (PRIMARY CONTROLLER)
This must act as a **lightweight orchestrator layer** and include:
- Intent detection
- Complexity detection (simple vs complex)
- Requirement validation logic
- Mode definitions
- Transition rules
- Token efficiency principles
---
# 🔷 ADAPTIVE WORKFLOW (CRITICAL)
The system MUST support TWO execution paths:
---
## ⚡ FAST PATH (Simple Tasks)
Trigger when:
- Task is small, clear, and self-contained
Examples:
- Generate HTML
- Write a simple function
- Fix a bug
Behavior:
- Skip validation
- Skip refinement and spec
- Execute immediately
- Ask minimal clarification only if required
---
## 🧠 DEEP PATH (Complex Tasks)
Trigger when:
- Requirement is ambiguous OR
- Includes multiple components OR
- Requires architecture/design decisions
---
### Step 1 — Requirement Validation (ONLY for complex)
Use this checklist:
1. Clear objective
2. Acceptance criteria
3. Inputs/outputs defined
4. Technical/functional context
5. Edge cases considered
Rules:
- ≥ 4 → VALID ✅ → proceed
- < 4 → INVALID ❌ → improvement mode
---
### Requirement Improvement Mode
- Explain gaps
- Ask structured questions
- Suggest improvements
- Loop until requirement is valid
---
### Step 2 — Refinement Mode
- Break requirement into structured understanding
- Identify gaps
- Ask critical “grill” questions
---
### Step 3 — Specification Mode
Generate:
- Feature overview
- Functional requirements
- API/contracts
- Edge cases
- Acceptance criteria
---
### Step 4 — Approval Gate
- Wait for user confirmation
---
### Step 5 — Implementation Mode
- Break spec into tasks
- Generate clean, reusable code
- Follow best practices
---
### Step 6 — Validation Mode
- Compare code vs specification
- Identify risks
- Suggest improvements
- Generate unit tests
---
# 🔷 MODE-BASED DESIGN (NO EXPLICIT AGENTS)
Use MODES:
- Refinement → Analyst
- Specification → Architect
- Implementation → Developer
- Validation → Reviewer
Modes must:
- Activate automatically
- Be context-driven
- Avoid repetition
---
# 🔷 ORCHESTRATION LOGIC
1. Detect complexity FIRST:
   - SIMPLE → Fast Path
   - COMPLEX → Validation
2. Apply validation ONLY for complex tasks
3. Route execution accordingly
---
# 🔷 TOKEN EFFICIENCY RULES
- Do NOT repeat context
- Use conversation history
- Keep orchestration minimal
- Avoid explicit agent instructions
- Apply skills implicitly
- Skip unnecessary steps
---
# 🔷 SKILLS (IMPLICIT)
Include:
- Summarization
- Requirement analysis
- Code generation
- Validation
- Refactoring
- Test generation
Do NOT explicitly invoke them.
---
# 🔷 DELIVERABLES (MANDATORY)
Generate ALL of the following:
---
## ✅ 1. Full `copilot-instructions.md`
Include:
- Orchestrator layer
- Complexity detection
- Validation logic
- Modes
- Transitions
- Token efficiency rules
---
## ✅ 2. Recommended Repository Structure
Example:
.copilot/
  instructions/
  modes/
  skills/
  docs/
Explain each component briefly
---
## ✅ 3. Visual Diagrams (VERY IMPORTANT)
Use Mermaid OR clean structured diagrams:
### a) Workflow Diagram
User → Orchestrator → Complexity → Validation → Fast/Deep Path → Modes
### b) User Flow Diagram
User interaction loop with feedback and approval
### c) High-Level Architecture Diagram
Show:
- Copilot
- Instructions layer
- Orchestrator
- Modes
- Repo context
Ensure:
- Clean
- Professional
- Easy to understand
---
## ✅ 4. Example Scenarios
Provide:
### Example 1 — Simple Task
- HTML / small function
- Show Fast Path behavior
### Example 2 — Complex Poor Requirement
- Show validation failure
- Show improvement loop
### Example 3 — Complex Good Requirement
- Show full workflow
---
## ✅ 5. FULL MARKDOWN DOCUMENTATION FILE (VERY IMPORTANT)
Create a file:
# 📄 AI Engineering Pattern – Copilot Agentic Workflow
This markdown file must include:
## Sections:
### 1. Overview
- What this pattern is
- Why it is needed
### 2. Architecture
- Explain orchestrator
- Explain modes
- Explain adaptive flow
### 3. Workflow
- Step-by-step explanation
### 4. Diagrams
- Include ALL diagrams (Mermaid)
### 5. Execution Model
- Fast Path vs Deep Path
### 6. Requirement Validation
- Checklist-based approach
- JIRA alignment
### 7. Examples
- Simple
- Complex (poor + good)
### 8. Design Principles
- Token efficiency
- Instruction-driven design
- Scalability
### 9. How to Use
- How developer interacts with Copilot
### 10. Benefits
- Reduced prompts
- Faster development
- Better quality outputs
Ensure:
- Clean Markdown formatting
- Headings, sections, readability
- Ready to store in repo (docs folder)
---
# 🔷 CONSTRAINTS
- Keep practical and implementable
- Avoid over-engineering
- Ensure Copilot-native behavior
- No external orchestration tools
- Keep everything clean and minimal
---
# ✅ FINAL EXPECTATION
The output must be:
- Production-ready
- Cleanly structured
- Immediately usable
- Enterprise-friendly
- Includes diagrams + documentation
- Delivered as a reusable pattern
---
Start now.
