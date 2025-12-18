# Media Integration Guide

This guide explains how to add GIFs and images to the IBO Studio documentation.

## Directory Structure

Create an `images` folder in the `docs` directory to store your media files:

```
docs/
├── images/
│   ├── components/
│   │   ├── button-example.gif
│   │   ├── dropdown-usage.gif
│   │   ├── datefield-picker.gif
│   │   └── ...
│   ├── editor/
│   │   ├── drag-drop.gif
│   │   ├── properties-panel.gif
│   │   └── ...
│   └── workflows/
│       ├── create-form.gif
│       ├── connect-datasource.gif
│       └── ...
```

## Markdown Syntax for Images/GIFs

### Basic Image/GIF Embedding

```markdown
![Alt text description](images/components/button-example.gif)
```

### With Caption

```markdown
![Drag and drop components onto the canvas](images/editor/drag-drop.gif)
*Figure 1: Dragging a button component onto the canvas*
```

### Centered with HTML

```markdown
<div align="center">
  <img src="images/components/dropdown-usage.gif" alt="Dropdown usage example" width="600">
  <p><em>Using the Dropdown component with dynamic data binding</em></p>
</div>
```

## Best Practices for GIFs

### Recording Guidelines

1. **Resolution**: 1280x720 or 1920x1080 for clarity
2. **Frame Rate**: 10-15 fps is sufficient (keeps file size down)
3. **Duration**: Keep under 10-15 seconds per GIF
4. **Focus**: Show one specific action or workflow per GIF
5. **Cursor**: Make cursor visible for click actions

### Optimization

1. **File Size**: Keep under 5MB per GIF (use tools like Giphy, ezgif.com, or ffmpeg to compress)
2. **Looping**: Enable loop for instructional GIFs
3. **First Frame**: Make sure the first frame shows the initial state clearly

### Recording Tools

- **Windows**: ScreenToGif (free, excellent quality control)
- **Mac**: Kap, Gifski, or built-in QuickTime + converter
- **Online**: CloudApp, Loom (can export as GIF)

## Component Documentation Examples

### TextField Example

```markdown
## TextField

Text input component with validation and keyboard types.

![TextField in action](images/components/textfield-typing.gif)

### Usage

\`\`\`json
{
  "type": "TextField",
  "props": {
    "name": "email",
    "label": "Email Address",
    "keyboard": "email"
  }
}
\`\`\`

![Different keyboard types](images/components/textfield-keyboards.gif)
*The keyboard type automatically adapts based on the `keyboard` property*
```

### Dropdown with Data Binding

```markdown
## Dropdown

![Binding dropdown to data source](images/components/dropdown-datasource.gif)

1. Select the Dropdown component
2. Configure the data source in the properties panel
3. Map value and label keys
4. Preview updates in real-time
```

## Example Integration in components.md

Here's how you could enhance the existing component documentation:

```markdown
## Button + Submit Action

![Button click triggering form submission](images/components/button-submit.gif)

\`\`\`json
{
  "type": "Button",
  "props": {
    "text": "Submit",
    "action": {
      "type": "submit",
      "url": "https://api.example.com/orders"
    }
  }
}
\`\`\`

**Watch the GIF above to see:**
1. User fills out the form
2. Clicks the Submit button
3. Data is sent to the API
4. Success message appears
```

## Workflow Documentation with GIFs

For the Build Playbook, use GIFs to show complete workflows:

```markdown
## Creating Your First Form

Follow these steps to create a data entry form:

### Step 1: Add a Form Component

![Adding a form to the canvas](images/workflows/add-form-component.gif)

1. Click the "+" button in the component tree
2. Select "FormGrid" from the modal
3. The form appears on the canvas

### Step 2: Configure Fields

![Configuring form fields](images/workflows/configure-fields.gif)

Add and configure multiple fields through the properties panel.

### Step 3: Connect Data Source

![Connecting to API](images/workflows/connect-api.gif)

Link your form to a backend API for data submission.
```

## File Naming Conventions

Use descriptive, lowercase names with hyphens:

✅ Good:
- `dropdown-select-item.gif`
- `datefield-date-picker.gif`
- `form-submit-success.gif`

❌ Avoid:
- `GIF1.gif`
- `Screen Recording 2024.gif`
- `dropdown_example.gif` (use hyphens, not underscores)

## Troubleshooting

### GIF Not Showing

1. Check the file path is correct relative to the markdown file
2. Ensure the file extension is lowercase (`.gif` not `.GIF`)
3. Verify the image is in the correct directory

### GIF Too Large

Use compression tools:
```bash
# Using ffmpeg to optimize GIF
ffmpeg -i input.gif -vf "fps=10,scale=800:-1:flags=lanczos" -c:v gif output.gif
```

Or use online tools:
- https://ezgif.com/optimize
- https://www.iloveimg.com/compress-image/compress-gif

## Checklist for Adding GIFs

- [ ] Create `docs/images/` directory structure
- [ ] Record screen at appropriate resolution
- [ ] Edit/trim to show only relevant action (10-15 seconds max)
- [ ] Optimize file size (aim for under 3-5MB)
- [ ] Use descriptive filename
- [ ] Add to appropriate subfolder
- [ ] Embed in markdown with descriptive alt text
- [ ] Add caption or explanation
- [ ] Test in generated documentation site
- [ ] Commit images to repository

## Next Steps

1. Set up the `docs/images/` directory structure
2. Record GIFs for your priority components
3. Start with the most complex or commonly used components
4. Update component documentation progressively
