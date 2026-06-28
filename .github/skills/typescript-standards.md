# Skill: TypeScript Standards

**Trigger**: Apply these rules whenever writing or reviewing TypeScript code.

**Rules**:
1. **Strict Typing**: Avoid `any`. Use `unknown` if the type is truly dynamic, and use type guards.
2. **Interfaces over Types**: Prefer `interface` for object shapes, use `type` for unions and primitives.
3. **Functional Patterns**: Prefer immutability. Use `.map()`, `.filter()`, and `.reduce()` over `for` loops.
4. **Error Handling**: Use `try/catch` with typed errors. Do not swallow exceptions silently.
5. **Exports**: Use named exports instead of default exports to ensure consistent naming across the codebase.
