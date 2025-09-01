# Contributing to TikTok Gift Tracker

Thank you for your interest in contributing to the TikTok Gift Tracker! This guide will help you get started with contributing to the project.

## 🚀 Getting Started

### Prerequisites
- Basic knowledge of HTML, CSS, and JavaScript
- A web browser for testing
- Git for version control
- A text editor or IDE

### Setting Up the Development Environment

1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/tiktok-gift-tracker.git
   cd tiktok-gift-tracker
   ```

2. **Create a new branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Start development**
   - Open `index.html` in your browser
   - Or use a local server: `python -m http.server 8000`

## 📋 How to Contribute

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates.

**When submitting a bug report, please include:**
- A clear, descriptive title
- Steps to reproduce the issue
- Expected vs actual behavior
- Screenshots if applicable
- Browser and version information
- Console errors (if any)

### Suggesting Enhancements

Enhancement suggestions are welcome! Please include:
- A clear description of the enhancement
- The motivation/use case for the enhancement
- Any implementation ideas you might have

### Pull Requests

1. **Follow the existing code style**
   - Use consistent indentation (2 spaces)
   - Follow existing naming conventions
   - Add comments for complex logic

2. **Test your changes**
   - Test in multiple browsers (Chrome, Firefox, Safari)
   - Test responsive design on different screen sizes
   - Verify WebSocket connection still works

3. **Update documentation**
   - Update README.md if you add new features
   - Add inline comments for complex code
   - Update this CONTRIBUTING.md if you change the development process

4. **Commit messages**
   ```
   feat: add new gift animation effect
   fix: resolve connection timeout issue
   docs: update installation instructions
   style: improve mobile responsive design
   refactor: simplify gift tracking logic
   ```

## 🛠️ Development Guidelines

### Code Style

**HTML:**
- Use semantic HTML5 elements
- Maintain proper indentation
- Include appropriate ARIA labels for accessibility

**CSS:**
- Use CSS custom properties for theming
- Follow BEM methodology for class naming when adding new styles
- Ensure responsive design principles
- Use CSS Grid and Flexbox for layouts

**JavaScript:**
- Use modern ES6+ features
- Follow camelCase naming convention
- Use meaningful variable and function names
- Add error handling for network requests
- Use async/await for asynchronous operations

### File Structure
```
tiktok-gift-tracker/
├── index.html          # Main application file
├── README.md          # Project documentation
├── LICENSE            # MIT license
├── CONTRIBUTING.md    # This file
├── .gitignore        # Git ignore rules
└── package.json      # Project metadata
```

### Testing Guidelines

Since this is a client-side application, testing involves:

1. **Manual Testing**
   - Test all interactive elements (buttons, forms)
   - Verify animations work smoothly
   - Check responsive design on different screen sizes
   - Test WebSocket connection and disconnection

2. **Browser Compatibility**
   - Chrome (latest 2 versions)
   - Firefox (latest 2 versions)  
   - Safari (latest 2 versions)
   - Edge (latest 2 versions)

3. **Performance Testing**
   - Monitor memory usage during long sessions
   - Verify smooth animations at 60fps
   - Test with many rapid gift events

## 🎨 Design Guidelines

### Visual Design
- Maintain the glassmorphic design aesthetic
- Use the existing color palette consistently
- Ensure sufficient contrast for accessibility
- Keep animations smooth and purposeful

### User Experience
- Prioritize clarity and readability
- Maintain intuitive navigation
- Provide clear feedback for user actions
- Ensure the interface works well on mobile devices

### Animation Guidelines
- Use CSS transforms for performance
- Keep animations under 300ms for micro-interactions
- Use easing functions for natural movement
- Avoid animations that could trigger seizures

## 🐛 Common Issues and Solutions

### WebSocket Connection Issues
- Ensure the server URL format is correct
- Check for CORS issues if testing locally
- Verify API key format and authentication

### Performance Issues  
- Monitor DOM manipulation efficiency
- Use `requestAnimationFrame` for smooth animations
- Avoid memory leaks in event listeners

### Styling Issues
- Test CSS changes across different browsers
- Ensure mobile responsiveness
- Maintain design consistency

## 📝 Documentation

When adding new features, please update:
- README.md with usage instructions
- Inline code comments
- JSDoc comments for functions
- Configuration examples

## 🏆 Recognition

Contributors will be recognized in the following ways:
- Listed in the README.md contributors section
- GitHub contributor statistics
- Release notes mentions for significant contributions

## ❓ Questions?

If you have questions about contributing:
1. Check existing issues and discussions
2. Create a new issue with the "question" label
3. Reach out to maintainers

## 📄 Code of Conduct

Please be respectful and constructive in all interactions. We aim to create a welcoming environment for all contributors.

Thank you for contributing to the TikTok Gift Tracker! 🎉
