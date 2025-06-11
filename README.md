# AleLabs Blog Documentation

This documentation provides guidelines for developers on how to maintain and update the AleLabs blog content.

## Table of Contents
- [Project Structure](#project-structure)
- [Adding a New Blog Post](#adding-a-new-blog-post)
- [Updating Existing Content](#updating-existing-content)
- [Styling Guidelines](#styling-guidelines)
- [Image Guidelines](#image-guidelines)
- [Technical Requirements](#technical-requirements)

## Project Structure

```
site/
├── index.html          # Main blog page containing all posts
├── css/               # Stylesheets
│   └── bootstrap.min.css
├── js/                # JavaScript files
│   ├── jquery-1.11.3.min.js
│   └── bootstrap.min.js
├── logo.jpg           # Site logo and favicon
└── README.md          # This documentation file
```

## Adding a New Blog Post

To add a new blog post, follow these steps:

1. Open `index.html` and locate the `<div class="content">` section
2. Add a new `<article>` element with a unique ID following this template:

```html
<article id="your-post-id" class="blog-post">
    <h1>Your Blog Post Title</h1>
    <p class="blog-meta">Publication Date | Category | Written by Felix, Technician and Owner at AleLabs Tech</p>

    <!-- Introduction -->
    <p>Your introduction paragraph here...</p>

    <!-- Main Content -->
    <h2>First Section Title</h2>
    <p>Section content...</p>

    <h3>Subsection Title</h3>
    <ul>
        <li>List item 1</li>
        <li>List item 2</li>
    </ul>

    <!-- Conclusion -->
    <h2>Conclusion</h2>
    <p>Concluding paragraph...</p>
</article>
```

3. Add a navigation link in the sidebar:
```html
<li><a href="#your-post-id">Your Blog Post Title</a></li>
```

### Post Structure Guidelines

- Use semantic HTML5 elements (`<article>`, `<section>`, etc.)
- Include a unique ID for each post (use kebab-case)
- Follow the established heading hierarchy (h1 → h2 → h3)
- Include the standard meta information (date, category, author)
- Use appropriate HTML elements for content:
  - `<ul>` or `<ol>` for lists
  - `<p>` for paragraphs
  - `<strong>` for emphasis
  - `<a>` for links

## Updating Existing Content

### Modifying a Post

1. Locate the post using its ID in the sidebar navigation
2. Find the corresponding `<article>` element
3. Make your changes while maintaining the HTML structure
4. Update the post's meta information if necessary

### Best Practices for Updates

- Keep the author attribution consistent
- Maintain the established formatting
- Update the publication date if making significant changes
- Test the page after updates to ensure proper rendering
- Check that the sidebar navigation still works correctly

## Styling Guidelines

The blog uses Bootstrap for responsive design. Key styling classes:

- `blog-post`: Main container for each post
- `blog-meta`: Post metadata styling
- `content`: Main content area
- `sidebar`: Navigation sidebar

### Custom CSS Classes

```css
.blog-post {
    margin-bottom: 60px;
    padding: 30px;
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 15px rgba(0,0,0,0.1);
}

.blog-meta {
    color: #666;
    margin-bottom: 20px;
}

.sidebar {
    position: fixed;
    width: 280px;
    height: 100vh;
    background: #1a252f;
    padding: 30px;
    color: white;
}
```

## Image Guidelines

When adding images to blog posts:

1. Use the `<img>` tag with appropriate attributes:
```html
<img src="path/to/image.jpg" alt="Descriptive alt text" class="blog-image">
```

2. Image requirements:
- Format: JPG or PNG
- Maximum width: 800px
- Alt text: Descriptive and meaningful
- Class: Use `blog-image` for consistent styling

## Technical Requirements

- HTML5
- CSS3
- Bootstrap 4
- jQuery 1.11.3
- Responsive design support
- Cross-browser compatibility

### Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS/Android)

## Maintenance Tasks

Regular maintenance should include:

1. Checking and updating links
2. Verifying responsive design
3. Testing navigation functionality
4. Updating Bootstrap and jQuery if needed
5. Optimizing images
6. Checking browser compatibility

## Contact

For technical support or questions about the blog:
- Email: customers@alelabs.com
- Phone: +250 788612171

---

*Last updated: March 2024* 