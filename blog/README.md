# Blog Setup Instructions

## How to Add a New Blog Post

### Quick Method (Recommended)

1. **Copy the template:**
   ```bash
   cp post-template.html my-new-post.html
   ```

2. **Edit the file:**
   - Change `POST_TITLE` in the `<title>` tag and `<h1>` tag
   - Update `DATE` in the post-meta section
   - Add your content in the content area
   - Save the file

3. **Add to blog index:**
   - Open `blog/index.html`
   - Replace the "No blog posts yet" section with your new post:
   ```html
   <div class="blog-post">
       <div class="post-header">
           <h2 class="post-title"><a href="my-new-post.html">My Post Title</a></h2>
           <div class="post-meta">
               <span class="post-date">January 1, 2025</span>
               <div class="post-tags">
                   <span class="tag">Tech</span>
                   <span class="tag">AI</span>
               </div>
           </div>
       </div>
       <p class="post-excerpt">Short description of your post...</p>
       <a href="my-new-post.html" class="read-more">Read More</a>
   </div>
   ```

4. **Commit and push:**
   ```bash
   git add .
   git commit -m "Add new blog post: My Post Title"
   git push
   ```

### File Structure

```
vohvelikissa.github.io/
├── index.html          # Your homepage
├── blog/
│   ├── index.html      # Blog listing page
│   ├── post-template.html  # Template for new posts
│   ├── my-first-post.html   # Example post
│   ├── my-second-post.html  # Example post
│   └── README.md       # This file
└── pessi.jpg           # Your profile image
```

### Tips for Great Blog Posts

1. **Use clear titles** - Make them descriptive and engaging
2. **Add dates** - Helps readers understand when content was written
3. **Use tags** - Helps organize your content (Tech, AI, Development, etc.)
4. **Keep it readable** - Use paragraphs, headings, and lists
5. **Add images** - Visual content makes posts more engaging
6. **Use code blocks** - For technical content, use `<pre><code>` tags

### Styling Notes

- All styling matches your main homepage design
- Colors, fonts, and spacing are consistent
- Responsive design works on mobile and desktop
- Navigation links between home and blog

### Example Post Structure

```html
<!-- In your post file -->
<h1>My Awesome Post</h1>

<div class="post-meta">
    <span>📅 January 1, 2025</span>
    <span>✍️ Pessi Vilppolahti</span>
</div>

<p>This is my first paragraph...</p>

<h2>Section Heading</h2>
<p>More content here...</p>

<h3>Subsection</h3>
<p>Even more content...</p>

<pre><code>
// Code example
function hello() {
    return "World";
}
</code></pre>

<blockquote>
    This is a quote that stands out
</blockquote>

<p><a href="https://example.com">Link to something</a></p>
```

### Publishing

Your blog will be automatically available at:
```
https://vohvelikissa.github.io/blog/
```

Individual posts will be at:
```
https://vohvelikissa.github.io/blog/my-new-post.html
```
