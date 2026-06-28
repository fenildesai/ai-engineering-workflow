# Prompt: Pull Request Review

**Usage**: Use this prompt when asked to review a diff or a set of staged changes.

**Structure**:
1. **Summary**: Provide a 2-sentence summary of what the PR accomplishes.
2. **Logic & Correctness**: Are there any bugs, off-by-one errors, or incorrect assumptions?
3. **Code Quality**: Does the code adhere to our `.github/skills/` guidelines? 
4. **Testing**: Are there tests included? Do they cover the necessary edge cases?
5. **Verdict**: Approve, Request Changes, or Comment.
