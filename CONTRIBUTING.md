# Contributing to Totally Free APIs

Thank you for your interest in contributing to Totally Free APIs! This guide will help you understand how to contribute effectively.

## 🎯 Our Mission

We curate **completely free APIs that require no authentication** for indie developers with zero budget. Quality over quantity is our principle.

## 📋 API Inclusion Criteria

Before submitting an API, please ensure it meets ALL of the following criteria:

### ✅ Required Criteria
- **Completely Free**: No hidden costs, premium tiers, or paid features
- **No Authentication**: No API keys, tokens, registration, or authentication required
- **Stable & Production-Ready**: Not a test/demo API, actively maintained
- **Well-Documented**: Has clear documentation and usage examples
- **HTTPS Support**: Supports secure connections
- **Reliable**: Has good uptime and performance

### ❌ Exclusion Criteria
- APIs requiring any form of authentication (API keys, OAuth, etc.)
- Freemium APIs (free tier with paid upgrades)
- Test/demo/beta APIs
- APIs with rate limits too restrictive for practical use
- APIs requiring credit card information for registration
- Unstable or frequently offline APIs

## 📝 How to Contribute

### 1. Fork the Repository
Click the "Fork" button at the top right of this repository.

### 2. Add Your API
Edit the `README.md` file and add your API to the appropriate category:

```markdown
| API Name | Description | HTTPS | Link |
|----------|-------------|-------|------|
| Your API | Brief description | ✅ | [Go!](https://your-api.com/) |
```

### 3. Category Guidelines
- Place APIs in the most appropriate existing category
- If no suitable category exists, suggest a new one in your PR description
- Keep descriptions concise but informative (under 50 characters)

### 4. Testing Your API
Before submitting, please test the API:
```bash
# Example test
curl "https://your-api.com/endpoint"
```

### 5. Submit a Pull Request
- Use a descriptive title: "Add [API Name] - [Brief Description]"
- Include the following in your PR description:
  - API endpoint example
  - Brief explanation of what the API does
  - Confirmation that it meets all criteria

## 📐 Pull Request Template

```markdown
## API Information
- **Name**: [API Name]
- **URL**: [API URL]
- **Category**: [Proposed Category]
- **Description**: [What does this API do?]

## Verification Checklist
- [ ] API is completely free
- [ ] No authentication required
- [ ] HTTPS supported
- [ ] Well documented
- [ ] Tested and working
- [ ] Production-ready (not test/demo)

## Example Usage
```bash
curl "https://api.example.com/endpoint"
```

## Additional Notes
[Any additional information about the API]
```

## 🔍 Review Process

1. **Automated Checks**: We may run automated tests on submitted APIs
2. **Manual Review**: Maintainers will verify the API meets our criteria
3. **Community Feedback**: The community may provide feedback on submissions
4. **Approval**: Once approved, your API will be merged

## 🚫 Common Rejection Reasons

- API requires authentication
- API is freemium (has paid tiers)
- API is unstable or frequently offline
- Poor or missing documentation
- Test/demo API not intended for production use
- Duplicate submission

## 🛠️ Maintenance

### Reporting Broken APIs
If you find an API that no longer works or has changed its terms:
1. Open an issue with the title "Broken API: [API Name]"
2. Provide details about what's broken
3. Suggest whether it should be removed or updated

### Updating Existing APIs
- Submit a PR with updated information
- Explain what changed and why the update is needed

## 💡 Suggestions for New Categories

We welcome suggestions for new API categories. When proposing a new category:
- Ensure there are at least 3-5 APIs that would fit
- Choose a clear, descriptive category name
- Provide reasoning for why a new category is needed

## 🎨 Style Guidelines

- Use emoji icons for categories (📍 🎲 🌤️ etc.)
- Keep descriptions concise and informative
- Use consistent formatting in tables
- Maintain alphabetical order within categories when possible

## 📞 Getting Help

- **Questions**: Open an issue with the "question" label
- **Discussions**: Use GitHub Discussions for broader topics
- **Problems**: Open an issue with the "help wanted" label

## 🏆 Recognition

Contributors will be recognized in our documentation. Significant contributors may be invited to become maintainers.

---

**Thank you for helping build the best collection of truly free APIs for indie developers!** 🚀 