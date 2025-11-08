# Contributing to Aabha ESlint Plugin

Thank you for your interest in contributing to Aabha! We welcome contributions from the community.

## Table of Contents

- [Contributing to Aabha ESlint Plugin](#contributing-to-aabha-eslint-plugin)
  - [Table of Contents](#table-of-contents)
  - [Code of Conduct](#code-of-conduct)
    - [Our Pledge](#our-pledge)
    - [Our Standards](#our-standards)
  - [How Can I Contribute?](#how-can-i-contribute)
  - [Documentation Contributions](#documentation-contributions)
    - [Finding Documentation to Complete](#finding-documentation-to-complete)
    - [Documentation Structure](#documentation-structure)
    - [OgPgy Bank Examples](#ogpgy-bank-examples)
    - [Areas for Code Contributions](#areas-for-code-contributions)
    - [Code Style](#code-style)
  - [Development Setup](#development-setup)
    - [Prerequisites](#prerequisites)
    - [Setup Steps](#setup-steps)
  - [Style Guidelines](#style-guidelines)
    - [Documentation Style](#documentation-style)
    - [Code Style](#code-style-1)
  - [Recognition](#recognition)
  - [Questions?](#questions)
  - [License](#license)

## Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inspiring community for all. Please be respectful and constructive in your interactions.

### Our Standards

**Examples of behavior that contributes to a positive environment:**
- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community
- Showing empathy towards other community members

**Examples of unacceptable behavior:**
- Trolling, insulting/derogatory comments, and personal or political attacks
- Public or private harassment
- Publishing others' private information without explicit permission
- Other conduct which could reasonably be considered inappropriate

## How Can I Contribute?

## Documentation Contributions

### Finding Documentation to Complete

All incomplete documentation files are marked with:

```markdown
> **📝 Documentation In Progress**
>
> This guide is currently being developed. We welcome contributions!
```

### Documentation Structure

Each API reference should include:

1. **Overview** - What it does, why it matters
2. **Import** - How to import
3. **Parameters** - Complete parameter reference with types
4. **Examples** - 2-3 real-world examples (use OgPgy Bank characters)
5. **Common Patterns** - Typical usage patterns
6. **Validation Rules** - What TypeScript enforces
7. **Best Practices** - Do's and don'ts
8. **See Also** - Links to related docs

### OgPgy Bank Examples

When creating examples, use characters from `examples/ogpgy-bank/BACKSTORY.md` from `aabha`:

### Areas for Code Contributions

1. **New Decorators** - If you identify a gap in the hierarchy
2. **Decorator Options** - Additional configuration options
3. **Type Utilities** - Helper types for better DX
4. **Validation** - Improved compile-time checks
5. **Error Messages** - Clearer error messages

### Code Style

- Follow existing TypeScript conventions
- Use meaningful variable names
- Add JSDoc comments for public APIs
- Include type annotations
- Write tests for new functionality

## Development Setup

### Prerequisites

- Node.js 18+
- pnpm (recommended) or npm/yarn
- TypeScript 5.0+

### Setup Steps

1. **Fork the repository**

   Visit [github.com/krabhishek/aabha](https://github.com/krabhishek/eslint-plugin-aabha) and click "Fork"

2. **Clone your fork**

   ```bash
   git clone https://github.com/YOUR_USERNAME/eslint-plugin-aabha.git
   cd aabha
   ```

3. **Install dependencies**

   ```bash
   pnpm install
   ```

4. **Build the project**

   ```bash
   pnpm run build
   ```

5. **Run type checking**

   ```bash
   pnpm run typecheck
   ```

6. **Create a branch**

   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b docs/api-context-decorator
   ```

## Style Guidelines

### Documentation Style

**Markdown:**
- Use proper heading hierarchy (# → ## → ###)
- Include code fences with language (```typescript)
- Use tables for structured data
- Add links to related documentation
- Include "See Also" sections

**Tone:**
- Professional but friendly
- Clear and concise
- Use examples liberally
- Avoid jargon (or explain it)

**Examples:**
- Use OgPgy Bank characters
- Show complete, runnable code
- Include comments explaining key points
- Demonstrate both ✅ good and ❌ bad patterns

### Code Style

**TypeScript:**
```typescript
// Use descriptive names
@Strategy({
  name: 'Digital-First Banking',  // Clear, descriptive
  whereToPlay: ['Young adults'],
  howToWin: 'Fastest onboarding'
})
class DigitalFirstStrategy {}  // Class name matches concept

// Add JSDoc for public APIs
/**
 * Defines a business strategy with WHERE to play and HOW to win.
 *
 * @example
 * ```typescript
 * @Strategy({
 *   name: 'Market Leadership',
 *   whereToPlay: ['Enterprise', 'SMB'],
 *   howToWin: 'Best developer experience'
 * })
 * class MarketLeadershipStrategy {}
 * ```
 */
export function Strategy(options: StrategyOptions) {
  // Implementation
}
```

**File Naming:**
- Use kebab-case for files: `context.decorator.ts`
- Use PascalCase for classes: `DigitalFirstStrategy`
- Match decorator names: `@Context` → `context.decorator.ts`

## Recognition

Contributors will be recognized in:
- Project README
- Release notes
- Contributors page (coming soon)

## Questions?

- **Documentation questions**: Open an issue with label `documentation`
- **Code questions**: Open an issue with label `question`
- **General discussion**: Use [GitHub Discussions](https://github.com/krabhishek/aabha/discussions)

## License

By contributing to Aabha, you agree that your contributions will be licensed under the MIT License.

---

**Thank you for contributing to Aabha!** 🙏

Every contribution, no matter how small, helps make context engineering more systematic and AI-assisted development more efficient.

The aura of a great product comes from clarity, and your contributions help bring clarity to context engineering everywhere.
