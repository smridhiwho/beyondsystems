# Beyond Systems Roadmap

This directory contains structured learning content for AI Engineering and Software Development.

## Directory Structure

```
roadmap/
├── index.html              # Main AI Engineering Roadmap (existing)
├── software-engineering.html   # NEW: Software Engineering Fundamentals overview
├── llm-api.html              # NEW: LLM API Guide overview
├── software-engineering/
│   └── 01-virtual-environments.html  # NEW: Lesson page template
└── llm-api/
    └── 01-api-fundamentals.html      # NEW: Lesson page template
```

## Adding New Content

### Adding a New Section Page

1. Copy `software-engineering.html` or `llm-api.html`
2. Rename to your new section name (e.g., `frontend.html`)
3. Update the title, description, and lesson cards
4. Update the hero section styling if needed

### Adding a New Lesson Page

1. Copy an existing lesson (e.g., `01-virtual-environments.html`)
2. Rename to the next number in the series (e.g., `02-package-management.html`)
3. Update the content
4. Update navigation links

### Adding to Section Overview Pages

Edit the `<article class="lesson-grid">` section in your section HTML file to add new lesson cards using the same pattern:

```html
<article class="lesson-card">
  <h3 class="lesson-title"><a href="XX-your-lesson-slug">Your Lesson Title</a></h3>
  <div class="lesson-meta">
    <span class="lesson-badge">Beginner</span>
    <span class="lesson-badge">20 min</span>
  </div>
  <p class="lesson-description">Brief description of what's covered.</p>
  <div class="lesson-tags">
    <span class="tag">#tag1</span>
    <span class="tag">#tag2</span>
  </div>
</article>
```

## Maintaining Good System Design

1. **Separation of Concerns**: Each HTML file is self-contained with its own styles and content
2. **Consistent Navigation**: All pages have the same topbar navigation
3. **SEO-Friendly**: Each page has proper meta tags and canonical URLs
4. **Mobile Responsive**: CSS includes mobile breakpoints
5. **Component-Based**: Reusable patterns for lesson cards, badges, and tags

## Integration Points

- Navigation links are relative (e.g., `../software-engineering.html`)
- CSS is embedded per page for offline viewing
- Analytics and Ads can be added via the header section

## Future Expansion Ideas

1. Add JavaScript for interactive elements (toc scroll, progress tracking)
2. Create JSON data files for dynamic content
3. Add dark/light mode toggle
4. Implement search functionality