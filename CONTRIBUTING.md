# Contributing to TFT Team Builder

Thank you for your interest in contributing to TFT Team Builder! We welcome contributions from the community.

## How Can I Contribute?

### 1. Report Bugs 🐛
Found a bug? Let us know!

**Before submitting:**
- Check if the issue already exists
- Try clearing your browser cache
- Test in a different browser

**When submitting:**
- Describe the bug clearly
- Steps to reproduce
- Browser and OS
- Expected vs actual behavior
- Screenshots if helpful

### 2. Suggest Enhancements 💡
Have an idea to improve the app?

**Before suggesting:**
- Check if it's already been suggested
- Make sure it aligns with the project vision

**When suggesting:**
- Explain the enhancement clearly
- Why would this be useful?
- How should it work?
- Any alternative approaches?

### 3. Update Game Data 📊
Help keep the meta data current!

**Data contributions:**
- New champions for upcoming sets
- Updated win rates and pick rates
- New meta compositions
- Balance changes
- Trait adjustments

**How to contribute data:**
1. Get the data from reliable sources (Mobalytics, patch notes, etc.)
2. Edit `index.html` - find the `tftData` object in the `<script>` section
3. Add or update the data structure
4. Test in your browser
5. Submit a pull request

### 4. Improve Documentation 📚
- Fix typos or unclear explanations
- Add examples or clarifications
- Improve README or guides
- Translate documentation

### 5. Code Improvements ⚙️
- Performance optimizations
- Bug fixes
- UI/UX improvements
- Accessibility enhancements
- Mobile optimization

---

## Development Setup

### Clone the Repository
```bash
git clone https://github.com/yourusername/tft-team-builder.git
cd tft-team-builder
```

### Open Locally
```bash
# Option 1: Direct open
open index.html

# Option 2: Local server
python -m http.server 8000
# Visit: http://localhost:8000
```

### Test Changes
1. Make your changes to `index.html`
2. Save the file
3. Refresh your browser
4. Test thoroughly
5. Clear cache if needed

---

## Making Changes

### Code Style
- Use consistent indentation (2 spaces)
- Use meaningful variable names
- Add comments for complex logic
- Keep functions focused and small

### HTML Structure
```html
<!-- Good: Clear, semantic structure -->
<div class="card">
    <h2>Title</h2>
    <p>Content</p>
</div>
```

### CSS Style
```css
/* Good: Organized, commented */
.card {
    background: rgba(0, 0, 0, 0.4);
    border: 1px solid rgba(34, 211, 238, 0.3);
    padding: 1.5rem;
}
```

### JavaScript Style
```javascript
// Good: Clear, purposeful code
function addUnit(unit) {
    if (currentTeam.length < 8) {
        currentTeam.push({ ...unit });
        renderTeamGrid();
    }
}
```

---

## Data Format Reference

### Adding a Champion
```javascript
{
    id: "champion-id",
    name: "Champion Name",
    cost: 4,
    traits: ["Trait1", "Trait2"],
    img: "🎭"  // Use emoji or icon
}
```

### Adding a Trait
```javascript
{
    name: "TraitName",
    description: "What this trait does"
}
```

### Adding a Meta Comp
```javascript
{
    id: "comp-id",
    name: "Comp Name",
    rating: "S",  // S, A, B, C
    winRate: 54.2,  // Percentage
    pickRate: 18.5,  // Percentage
    units: ["Unit1", "Unit2", "Unit3"],
    description: "Strategy description"
}
```

### Adding a New Set
```javascript
{
    id: "set18",
    name: "Set 18: Name",
    number: 18,
    status: "upcoming",  // current, legacy, upcoming
    releaseDate: "2025-08-21",
    units: [ ... ],
    traits: [ ... ],
    metaComps: [ ... ]
}
```

---

## Testing Your Changes

### Browser Compatibility
Test in:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

### Mobile Testing
- Test on actual device if possible
- Use browser dev tools device emulation
- Check touch interactions
- Verify responsive layout

### Feature Testing
- Team building works
- Saving/loading teams works
- Offline functionality works
- Meta data displays correctly
- All tabs function properly

---

## Submitting Changes

### Before You Submit
1. **Test thoroughly** - Make sure everything works
2. **Check existing PRs** - Don't duplicate work
3. **Update docs** - If you changed functionality
4. **Keep changes focused** - One feature per PR

### Creating a Pull Request

1. **Fork the repository**
```bash
git clone https://github.com/yourusername/tft-team-builder.git
```

2. **Create a feature branch**
```bash
git checkout -b feature/YourFeatureName
```

3. **Make your changes**
- Edit `index.html` (main file)
- Update `README.md` if needed
- Test thoroughly

4. **Commit your changes**
```bash
git add .
git commit -m "Add: Brief description of changes"
```

Good commit messages:
- Start with action: Add, Fix, Update, Improve
- Be specific and clear
- Example: "Add Set 16 champions and meta comps"

5. **Push to your fork**
```bash
git push origin feature/YourFeatureName
```

6. **Create Pull Request**
- Go to GitHub
- Click "New Pull Request"
- Select your branch
- Add title and description
- Include any relevant context
- Submit!

### PR Description Template
```markdown
## Description
Brief description of what this PR does.

## Changes
- Change 1
- Change 2
- Change 3

## Related Issues
Fixes #123

## Testing
- [ ] Tested in Chrome
- [ ] Tested in Safari
- [ ] Tested on mobile
- [ ] Data is correct

## Screenshots/Examples
If applicable, add screenshots.
```

---

## Review Process

### What We Look For
✅ Code is clean and understandable  
✅ Changes don't break existing features  
✅ Testing is thorough  
✅ Documentation is updated  
✅ Commits are meaningful  

### Feedback
- We'll review and provide feedback
- Ask questions if something isn't clear
- Work together to get it right
- Thank you for being patient!

---

## Community Guidelines

### Be Respectful
- Treat others with kindness
- Welcome diverse perspectives
- Assume good intentions
- Give and accept feedback gracefully

### Stay Focused
- Keep discussions relevant
- Stay on topic in issues/PRs
- Avoid off-topic comments

### No Spam
- Don't spam issues/PRs
- Don't promote unrelated products
- No self-promotion outside guidelines

---

## Areas We Need Help With

### High Priority
- ✅ Update Set 16/17 meta data
- ✅ Add new champion details
- ✅ Performance improvements
- ✅ Mobile optimization

### Medium Priority
- [ ] Add augment builder
- [ ] Item optimizer
- [ ] Better documentation
- [ ] UI improvements

### Nice to Have
- [ ] Translations
- [ ] Dark/light theme toggle
- [ ] Team export/import
- [ ] Share team links

---

## Questions?

### Getting Help
- Check existing issues
- Read the documentation
- Ask in new issues
- Comment on related PRs

### Contact
- Open an issue for public questions
- Be specific about your question
- Provide context and examples

---

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code.

**In short:**
- Be welcoming and inclusive
- Be respectful of differences
- Focus on what is best for the community
- Show empathy towards others

---

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

## Thank You! 🙏

We really appreciate your contributions! Whether it's code, data, documentation, or feedback, you're helping make TFT Team Builder better for everyone.

**Every contribution counts, no matter how small!**

---

<div align="center">

Made with ❤️ by the TFT Community

[Star us ⭐](https://github.com) | [Report Issues 🐛](https://github.com/issues) | [Request Features 💡](https://github.com/issues)

</div>
