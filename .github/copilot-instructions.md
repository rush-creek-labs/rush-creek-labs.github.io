# Copilot Instructions

## Code Review Guidelines

When reviewing code in this repository, please focus on providing high-value feedback that improves code quality, security, and maintainability.

### Primary Focus Areas

1. **Critical Security Issues**
   - Identify potential security vulnerabilities (e.g., XSS, injection attacks, exposed secrets)
   - Flag insecure data handling or authentication/authorization issues
   - Highlight use of deprecated or insecure dependencies
   - Check for hardcoded credentials or sensitive information

2. **Logic Bugs**
   - Identify logical errors that could cause incorrect behavior
   - Flag edge cases that aren't handled properly
   - Point out potential race conditions or concurrency issues
   - Highlight incorrect error handling or missing validations

### Review Style

- **Be concise and direct**: Provide clear, actionable feedback without unnecessary elaboration
- **Minimal emoji usage**: Limit emoji use to maintain a professional tone. Use sparingly (1-2 per review maximum)
- **Prioritize issues**: Focus on high-impact problems first. Don't flag minor style issues if there are more important concerns
- **Explain the why**: When identifying an issue, briefly explain why it's a problem and the potential impact
- **Suggest solutions**: Where possible, provide specific recommendations or code examples to fix issues

### Secondary Considerations

Only comment on these if no critical issues are found:

- Code maintainability and readability
- Performance optimizations (only if significant)
- Best practices and architectural improvements
- Test coverage for critical paths

### What to Avoid

- Nitpicking minor style preferences
- Commenting on formatting issues that linters should catch
- Excessive use of emojis or informal language
- Suggesting changes that don't meaningfully improve the code
- Flagging issues that are already handled by automated tools

## Repository-Specific Context

This is a GitHub Pages site for Rush Creek Labs LLC. The site is primarily static HTML with minimal JavaScript. When reviewing changes:

- Ensure any client-side code is secure and doesn't introduce XSS vulnerabilities
- Verify that external resources are loaded securely (HTTPS)
- Check that contact information and links are correct and functional
- Validate that responsive design and accessibility are maintained
