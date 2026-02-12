# Reclaim Tomorrow - Resource Library

A modern, responsive website for hosting PDFs and organizing progressive advocacy resources.

## Features

✅ **Multi-View Display**: Toggle between grid and list views
✅ **Advanced Search**: Real-time search across titles, descriptions, and tags
✅ **Smart Filtering**: Filter by topic, document type, and sort options
✅ **Mobile-Responsive**: Works beautifully on all devices
✅ **Clean Design**: Professional, progressive-themed aesthetic
✅ **Easy to Update**: Simple JavaScript data structure for adding resources

## Quick Start

1. **Upload the HTML file** to your web hosting service (GitHub Pages, Netlify, Vercel, etc.)
2. **Create a `resources` folder** in the same directory as the HTML file
3. **Add your PDF files** to the resources folder
4. **Update the resource data** in the JavaScript section (see below)

## Adding Your Resources

Open `reclaim-tomorrow.html` and find the `resources` array in the JavaScript section (around line 549). Each resource follows this structure:

```javascript
{
    id: 1,  // Unique number for each resource
    title: "Your Document Title",
    topic: "climate",  // Options: climate, healthcare, education, economy, justice, voting, housing, immigration
    type: "report",  // Options: report, factsheet, bibliography, policy, data
    date: "2024-01-15",  // Format: YYYY-MM-DD
    description: "Brief description of what this resource contains",
    tags: ["tag1", "tag2", "tag3"],  // Searchable keywords
    pdfUrl: "resources/your-file.pdf"  // Path to your PDF file
}
```

### Example: Adding a New Resource

```javascript
{
    id: 11,
    title: "Green New Deal: Implementation Guide",
    topic: "climate",
    type: "policy",
    date: "2024-02-12",
    description: "Step-by-step guide for implementing Green New Deal policies at local and state levels.",
    tags: ["green new deal", "climate policy", "implementation"],
    pdfUrl: "resources/green-new-deal-guide.pdf"
}
```

## Customization Options

### Changing Colors

Find the `:root` section in the CSS (around line 11) and modify these variables:

```css
--primary: #1a472a;        /* Main green color */
--accent: #e63946;         /* Red accent for buttons */
--light-bg: #f8f9fa;       /* Page background */
--card-bg: #ffffff;        /* Card backgrounds */
--text: #2d3436;          /* Main text color */
```

### Adding New Topics

1. Add the topic to the dropdown in the HTML:
```html
<option value="your-topic">Your Topic Name</option>
```

2. Add the label to the JavaScript `topicLabels` object:
```javascript
const topicLabels = {
    // ... existing topics ...
    yourtopic: "Your Topic Name"
};
```

### Adding New Document Types

Follow the same pattern as topics above for the `typeFilter` dropdown and `typeLabels` object.

### Changing Organization Name

Simply find and replace "Reclaim Tomorrow" in the HTML with your organization name.

## File Organization

```
your-website/
├── reclaim-tomorrow.html  (main website file)
└── resources/
    ├── climate-crisis.pdf
    ├── universal-healthcare.pdf
    ├── education-equity.pdf
    └── (all your other PDFs)
```

## Hosting Options

### Option 1: GitHub Pages (Free)
1. Create a GitHub repository
2. Upload your HTML file and resources folder
3. Enable GitHub Pages in repository settings
4. Your site will be at: `username.github.io/repository-name`

### Option 2: Netlify (Free)
1. Drag and drop your folder to netlify.com
2. Get instant deployment with custom domain support

### Option 3: Vercel (Free)
1. Import your GitHub repository
2. Automatic deployments on every update

### Option 4: Traditional Web Hosting
Upload files via FTP to any web hosting service.

## Browser Compatibility

✅ Chrome, Firefox, Safari, Edge (latest versions)
✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Tips for Best Results

1. **Optimize PDFs**: Compress large PDFs before uploading
2. **Consistent Naming**: Use clear, descriptive filenames (lowercase, hyphens instead of spaces)
3. **Regular Updates**: Date your resources and keep them current
4. **Descriptive Tags**: Use 3-5 relevant tags per resource for better searchability
5. **Mobile Testing**: Always test on mobile devices

## Accessibility Features

- Semantic HTML structure
- High contrast colors
- Keyboard navigation support
- Screen reader friendly
- Responsive text sizing

## Future Enhancements

Consider adding:
- Analytics tracking (Google Analytics)
- Contact form integration
- Newsletter signup
- Social sharing buttons
- Print stylesheets
- Dark mode toggle

## Support

For questions or issues:
1. Check the customization section above
2. Review the code comments in the HTML file
3. Search for similar questions online

## License

Free to use and modify for your organization's needs.

---

**Made for Reclaim Tomorrow** - Building a progressive future through informed advocacy.
# rctmrwbib
