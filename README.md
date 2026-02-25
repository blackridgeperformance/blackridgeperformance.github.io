# Blackridge Performance - Editing Guide

## How to Add/Edit Blog Posts

All blog posts are stored in `blog-posts.json`. You never need to touch the HTML files.

### Adding a New Post

1. Open `blog-posts.json`
2. Add a new entry at the top of the array (so it appears first):

```json
{
  "id": 4,
  "date": "MARCH 1, 2026",
  "title": "Your Post Title",
  "preview": "Short description that shows on the blog list page (2-3 sentences max)",
  "content": "Full article content goes here.\n\nUse \\n\\n to create new paragraphs.\n\nYou can write as much as you want here - it will be hidden until the user clicks to expand the post."
}
```

3. Make sure to add a comma after the previous entry
4. Increment the ID number for each new post

### Editing Existing Posts

Just edit the text in `blog-posts.json`. Changes will appear immediately when you refresh the blog page.

### Tips

- `\n\n` creates a paragraph break in the content
- Keep previews short - they're just teasers
- Date format: "MONTH DAY, YEAR" (all caps for month)
- ID numbers should be unique

### Example Structure

```json
[
  {
    "id": 1,
    "date": "FEBRUARY 25, 2026",
    "title": "Post Title",
    "preview": "Brief description",
    "content": "Full article text"
  },
  {
    "id": 2,
    "date": "FEBRUARY 20, 2026",
    "title": "Another Post",
    "preview": "Another description",
    "content": "More content"
  }
]
```

## Updating Site Updates

Edit `index.html` and find the Updates section. Add new entries like:

```html
<div class="update-entry">
  <div class="update-date">MAR 1, 2026</div>
  <p>Your update text here.</p>
</div>
```

## Changing Discord Username

In `index.html`, find:
```html
<div class="discord-username">YOUR_DISCORD_USERNAME</div>
```

Replace `YOUR_DISCORD_USERNAME` with your actual Discord username.

## File Structure

```
/
├── index.html          (main page)
├── blog.html           (blog page - don't edit this)
├── blog-posts.json     (edit this to add/change blog posts)
└── images/             (your car images)
    ├── 23209.png
    ├── car2.jpg
    ├── mycustombuild.png
    └── etrackbuild.jpg
```
