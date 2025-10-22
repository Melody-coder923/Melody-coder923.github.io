# Personal Website

This is my personal website built with Jekyll. It's designed for easy updates through markdown files.

## How to Update Content

### Resume
Edit `resume.md` in the root directory to update your resume. The file uses markdown formatting, so you can easily update:
- Education
- Skills
- Experience
- Projects

### Blog Posts
To add a new blog post:
1. Create a new markdown file in the `_posts` directory
2. Name it with the format: `YYYY-MM-DD-title-of-post.md`
3. Add the front matter at the top of the file:
   ```yaml
   ---
   layout: default
   title: "Your Post Title"
   date: YYYY-MM-DD
   ---
   ```
4. Write your post content in markdown below the front matter

### About Me
Edit `index.md` in the root directory to update your introduction and personal information.

## Local Development
To run the site locally:
```bash
jekyll serve --watch --livereload
```

## File Structure
```
.
├── _config.yml          # Site configuration
├── _layouts/            # HTML templates
├── _posts/             # Blog posts (add new .md files here)
├── index.md            # Homepage/About Me
├── resume.md           # Resume
└── blog.md             # Blog listing page
```