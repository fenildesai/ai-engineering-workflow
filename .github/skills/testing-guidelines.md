# Skill: Testing Guidelines

**Trigger**: Apply these rules whenever generating or reviewing tests.

**Rules**:
1. **Framework**: Assume Jest/Vitest and React Testing Library (if applicable) unless specified otherwise.
2. **Arrange-Act-Assert**: Structure all tests using the AAA pattern.
3. **Behavioral Testing**: Test the behavior and outputs, not the implementation details.
4. **Mocks**: Mock external API calls, databases, and heavy dependencies.
5. **Coverage**: Ensure tests cover the happy path, common error states, and edge cases defined in the requirement.
