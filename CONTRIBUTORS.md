# BLANK Browser Contributors

## How to Contribute to BLANK Browser

Thank you for your interest in contributing to BLANK Browser! We welcome contributions from designers, developers, security researchers, accessibility advocates, and community members.

---

## Getting Started

### Before You Contribute

1. **Read the [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)** - Familiarize yourself with our community standards
2. **Review [CONTRIBUTING.md](./CONTRIBUTING.md)** - Understand the process for submitting changes
3. **Check the [LICENSE](./LICENSE)** - Know that contributions go under MPL 2.0
4. **Read the [Design Philosophy](./design/concept-document.md)** - Understand BLANK's vision

### Types of Contributions We Welcome

#### 🎨 Design Contributions
- UI/UX improvements
- Visual design refinements
- Design system enhancements
- Accessibility improvements
- Color palette suggestions
- Typography refinements

#### 💻 Code Contributions
- Bug fixes
- New features (aligned with philosophy)
- Performance optimizations
- Code refactoring and cleanup
- Test coverage expansion
- Documentation improvements

#### 🔒 Security & Privacy
- Security vulnerability reports (private disclosure)
- Privacy audit findings
- Best practice recommendations
- Threat model analysis
- Encryption implementations

#### ♿ Accessibility
- WCAG 2.1 compliance improvements
- Screen reader testing
- Keyboard navigation enhancement
- Color contrast verification
- Focus management improvements

#### 📚 Documentation
- User guides and tutorials
- API documentation
- Design system documentation
- Keyboard shortcut guides
- Privacy explanations

#### 🧪 Testing & QA
- Bug discovery and reporting
- Performance testing
- Compatibility testing
- Cross-browser testing
- Edge case identification

#### 🌍 Localization
- Language translations
- Regional customizations
- Right-to-left (RTL) support
- Locale-specific testing

---

## How to Submit a Contribution

### Step 1: Fork the Repository

```bash
# Click "Fork" on GitHub
# Clone your fork locally
git clone https://github.com/[your-username]/blank-browser.git
cd blank-browser
```

### Step 2: Create a Feature Branch

```bash
# Create a branch with a descriptive name
git checkout -b feature/your-feature-name
# or
git checkout -b fix/bug-you-are-fixing
# or
git checkout -b docs/documentation-improvement
```

### Step 3: Make Your Changes

**For code**:
- Follow the code style (ESLint, Prettier)
- Write tests for new functionality
- Update documentation
- Keep commits atomic and well-described

**For design**:
- Use Figma for mockups
- Ensure WCAG 2.1 AAA compliance
- Include design rationale
- Test on multiple screen sizes

**For documentation**:
- Use clear, concise language
- Include examples
- Link to related sections
- Update table of contents if needed

### Step 4: Commit Your Changes

```bash
# Use descriptive commit messages
git commit -m "fix: Correct keyboard shortcut for tab navigation"
git commit -m "feat: Add dark mode toggle via Cmd+Shift+L"
git commit -m "docs: Update privacy architecture documentation"
git commit -m "test: Add tests for bookmark manager"
git commit -m "a11y: Improve screen reader announcements"
```

**Commit Message Format**:
```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `a11y`, `perf`

**Examples**:
- `feat(keyboard): Add Cmd+K command palette`
- `fix(privacy): Remove unintended data transmission`
- `docs(accessibility): Add WCAG compliance guide`
- `a11y(ui): Improve focus ring visibility`

### Step 5: Push to Your Fork

```bash
git push origin feature/your-feature-name
```

### Step 6: Create a Pull Request

1. Go to GitHub
2. Click "Compare & pull request"
3. Fill in the PR template with:
   - Description of changes
   - Why this change is needed
   - Any related issues (use `Closes #123`)
   - Testing performed
   - Accessibility compliance
   - Screenshots (if design/UI changes)

### Step 7: Respond to Review

- Be open to feedback
- Make requested changes
- Push updates to the same branch
- Respond to comments respectfully

### Step 8: Celebrate Your Contribution! 🎉

Once merged:
- Your name is added to the CONTRIBUTORS list
- You're credited in release notes
- Your changes benefit the community

---

## Contributor License Agreement (CLA)

By submitting a contribution to BLANK Browser, you agree that:

✅ **You own the copyright** to the code you're contributing (or have permission from the copyright holder)

✅ **You grant BLANK Browser rights** to use your contribution under the MPL 2.0 license

✅ **You grant patent rights** for any patents your contribution might infringe

✅ **Your contribution is original** and doesn't violate anyone else's rights

✅ **You understand** your contribution will be publicly available and used by others

---

## Recognition and Credits

### In-Code Attribution

For significant contributions, we'll add attribution:

```typescript
// Contributed by [Your Name] - [Year]
// Keyboard handler implementation with support for custom keybindings
```

### In Documentation

Your name appears in:
- [CONTRIBUTORS.md](./CONTRIBUTORS.md) (this file)
- Release notes
- Project README (for major contributions)
- GitHub contributors page

### Public Recognition

We celebrate contributors in:
- GitHub discussions
- Project announcements
- Community blog posts (if applicable)

---

## Code Style Guidelines

### TypeScript/JavaScript

```typescript
// ✅ Good: Clear, concise, well-typed
function handleKeyboardShortcut(
  event: KeyboardEvent,
  shortcuts: ShortcutMap
): void {
  const key = `${event.ctrlKey ? 'ctrl' : ''}+${event.key}`;
  const action = shortcuts.get(key);
  
  if (action) {
    action();
  }
}

// ❌ Avoid: Unclear, poorly typed
function handle(e, s) {
  let k = (e.ctrlKey ? 'ctrl' : '') + e.key;
  let a = s.get(k);
  if (a) a();
}
```

**Standards**:
- Use TypeScript for type safety
- Constant naming: `UPPER_SNAKE_CASE`
- Variable naming: `camelCase`
- Function naming: `camelCase` (start with verb for methods)
- File naming: `kebab-case.ts`
- Max line length: 100 characters
- Use descriptive variable names

### CSS/Styling

```css
/* ✅ Good: BEM naming, semantic */
.keyboard-handler__shortcut {
  padding: 8px 16px;
  background-color: var(--color-accent);
  border-radius: 4px;
}

.keyboard-handler__shortcut:hover {
  background-color: var(--color-accent-hover);
}

/* ❌ Avoid: Generic names, hard-coded colors */
.item { padding: 8px 16px; background: #0066cc; }
.item:hover { background: #0052a3; }
```

**Standards**:
- Use CSS custom properties for colors
- Follow 8px spacing grid
- Use BEM naming: `block__element--modifier`
- Provide clear focus states
- Ensure contrast ratios (7:1 minimum)

### Accessibility

```html
<!-- ✅ Good: Semantic, labeled, keyboard accessible -->
<button 
  aria-label="Open command palette"
  onClick={handleOpen}
  onKeyDown={handleKeyDown}
>
  Open Command Palette
</button>

<!-- ❌ Avoid: No label, not keyboard accessible -->
<div onClick={handleOpen}>Open</div>
```

**Standards**:
- Use semantic HTML (`<button>`, `<nav>`, `<main>`, etc.)
- Include ARIA labels where needed
- Ensure keyboard navigation works
- Test with screen readers
- Maintain 7:1 contrast ratio
- Clear focus indicators

---

## Testing

### Running Tests

```bash
# Run all tests
npm run test

# Run with coverage
npm run test -- --coverage

# Watch mode for development
npm run test -- --watch

# Accessibility tests
npm run test:a11y

# Performance tests
npm run test:performance
```

### Writing Tests

```typescript
describe('KeyboardHandler', () => {
  it('should execute Cmd+T shortcut for new tab', () => {
    const handler = new KeyboardHandler();
    const mockCallback = jest.fn();
    
    handler.register('Cmd+T', mockCallback);
    handler.handleKeyEvent(new KeyboardEvent('keydown', {
      metaKey: true,
      key: 't'
    }));
    
    expect(mockCallback).toHaveBeenCalled();
  });

  it('should not execute unregistered shortcuts', () => {
    const handler = new KeyboardHandler();
    const mockCallback = jest.fn();
    
    handler.handleKeyEvent(new KeyboardEvent('keydown', {
      metaKey: true,
      key: 'x'
    }));
    
    expect(mockCallback).not.toHaveBeenCalled();
  });
});
```

**Standards**:
- Write tests for all new features
- Aim for >80% code coverage
- Test edge cases
- Include accessibility tests
- Use descriptive test names

---

## Documentation Guidelines

### README Updates

Keep README.md updated with:
- New features
- Changed keyboard shortcuts
- Updated architecture
- New installation methods

### Code Comments

```typescript
// ✅ Good: Explains WHY not WHAT
// Skip macro shortcuts on special key combinations to avoid conflicts
// with system-level shortcuts (Cmd+Tab, Cmd+Q, etc.)
if (isSystemShortcut(key)) {
  return; // Let OS handle it
}

// ❌ Avoid: Obvious comments
// Increment i
i++;

// ❌ Avoid: Outdated comments
// This was broken in v0.5.2 but supposedly fixed
```

### Commit Messages

```
// ✅ Good: Clear, connected to issue
feat(keyboard): Add support for Vim keybindings

Allow users to enable Vim-style keyboard shortcuts through
preferences. Adds Vim motion commands to arrow keys.

Closes #234

// ❌ Avoid: Vague, no context
fixed stuff
```

---

## Community Guidelines

### Be Respectful

- Welcome people from all backgrounds
- Listen to different perspectives
- Assume good intent
- Address conflicts privately if possible
- Follow the [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)

### Share Knowledge

- Help newer contributors
- Explain your reasoning
- Link to relevant resources
- Share security/privacy expertise

### Give Constructive Feedback

```
// ✅ Good feedback
"I like this approach, but I'm concerned about performance
with large bookmark lists. Have you considered using
virtualization? See [link to example]."

// ❌ Avoid
"This is wrong."
```

### Accept Feedback

- Don't take critiques personally
- Ask clarifying questions
- Be willing to iterate
- Thank reviewers for their time

---

## Recognition of Contributors

### Core Team

- [Project Creator Name]
- [Add team members]

### Active Contributors

Listed alphabetically by GitHub username:

- [Will be populated as contributions grow]

### Special Thanks

To everyone who has:
- Reported bugs
- Suggested improvements
- Shared ideas
- Tested the browser
- Promoted BLANK Browser

---

## Questions?

### Getting Help

- **GitHub Issues**: Report bugs or ask questions
- **GitHub Discussions**: Discuss features and architecture
- **Contributing Guide**: See [CONTRIBUTING.md](./CONTRIBUTING.md)
- **Design Philosophy**: Read [Design Concepts](./design/concept-document.md)

### First-Time Contributors

We're excited to have you! Start with:

1. Look for [good-first-issue](https://github.com/[username]/blank-browser/labels/good-first-issue) tags
2. Read the feature documentation
3. Ask questions in GitHub Discussions
4. Submit your first PR with confidence

---

## Contribution Ideas

### High-Impact Areas

We're actively seeking contributions in:

- **Privacy auditing**: Review privacy architecture
- **Keyboard workflows**: Test and improve shortcuts
- **Accessibility testing**: Verify WCAG 2.1 AAA compliance
- **Documentation**: Explain features clearly
- **Performance**: Optimize rendering and memory
- **Security**: Find and report vulnerabilities
- **Design**: Refine UI/UX

### Growing the Community

Help BLANK Browser grow by:

- Writing tutorials about keyboard shortcuts
- Creating YouTube guides
- Testing on different systems
- Sharing your modifications
- Speaking about BLANK at conferences
- Writing blog posts about minimalist design

---

## Maintenance and Support

### How Long Do We Support Changes?

- **Bug fixes**: Supported until next major version
- **Features**: Maintained long-term
- **Security patches**: Applied to previous 2 versions minimum

### Deprecation Policy

If we need to remove features:
1. Announce deprecation (2 versions warning)
2. Provide migration guide
3. Support deprecated code for 2+ versions
4. Finally remove with major version bump

---

## License

By contributing to BLANK Browser, you agree your contributions are licensed under the [Mozilla Public License 2.0](./LICENSE).

Your contributions:
- Become part of BLANK Browser (with your attribution)
- Can be used by anyone under MPL 2.0 terms
- Remain your intellectual property (you retain copyright)
- Grant patent rights to the community

---

## Final Note

**Thank you for making BLANK Browser better!** Every contribution—code, design, ideas, feedback—makes a difference.

Together, we're building a browser that respects human agency, prioritizes privacy, and proves that simplicity and power aren't mutually exclusive.

---

*For more information, see [CONTRIBUTING.md](./CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)*

*Last updated: November 2, 2025*
