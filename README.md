# Jekyll Blog Setup for GitHub Pages

This repository contains your Care By Nurse website with integrated Jekyll blog functionality. The blog maintains the exact same design as your original website while providing a powerful content management system for daily blog posting.

## Features

- **Seamless Integration**: Blog functionality integrated into your existing website design
- **HTML Format**: All blog posts are in HTML format as requested
- **Responsive Design**: Works perfectly on desktop and mobile devices
- **GitHub Pages Ready**: Configured for automatic deployment on GitHub Pages
- **Sample Content**: Includes 3 sample blog posts to get you started

## Quick Start Guide

### 1. Setting Up GitHub Pages

1. **Create a GitHub Repository**:
   - Go to [GitHub.com](https://github.com) and create a new repository
   - Name it something like `care-by-nurse-website` or your preferred name
   - Make sure it's set to **Public** (required for free GitHub Pages)

2. **Upload Your Files**:
   - Upload all the files from this directory to your GitHub repository
   - You can do this by:
     - Using GitHub's web interface (drag and drop)
     - Using Git commands (if you're familiar with Git)
     - Using GitHub Desktop application

3. **Enable GitHub Pages**:
   - Go to your repository settings
   - Scroll down to "Pages" section
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

4. **Access Your Website**:
   - Your website will be available at: `https://yourusername.github.io/repository-name`
   - It may take a few minutes for the first deployment

### 2. Adding New Blog Posts Daily

Adding new blog posts is simple and can be done directly through GitHub's web interface:

#### Step-by-Step Process:

1. **Navigate to the _posts folder**:
   - Go to your GitHub repository
   - Click on the `_posts` folder

2. **Create a New File**:
   - Click "Add file" → "Create new file"
   - Name your file using this format: `YYYY-MM-DD-your-post-title.html`
   - Example: `2024-01-30-new-ndis-updates.html`

3. **Add the Post Content**:
   Copy and paste this template, then customize it:

```html
---
layout: post
title: "Your Blog Post Title Here"
date: 2024-01-30
author: "Your Name"
category: "Category Name"
featured_image: "img/your-image.jpg"
excerpt: "A brief description of your blog post that will appear in the blog listing."
---

<div class="post-content">
    <p>Your blog post content goes here. You can use HTML formatting.</p>
    
    <h2>Section Heading</h2>
    <p>More content here...</p>
    
    <h3>Subsection</h3>
    <p>Additional content...</p>
</div>
```

4. **Customize Your Post**:
   - **Title**: Replace "Your Blog Post Title Here" with your actual title
   - **Date**: Use today's date in YYYY-MM-DD format
   - **Author**: Your name or the author's name
   - **Category**: Choose from: "NDIS Support", "Daily Living", "Community", "Health Tips", "News", etc.
   - **Featured Image**: Path to an image in your img folder (optional)
   - **Excerpt**: A brief summary that appears on the blog listing page
   - **Content**: Write your blog post content using HTML

5. **Commit the File**:
   - Scroll down to "Commit new file"
   - Add a commit message like "Add new blog post: [Your Title]"
   - Click "Commit new file"

6. **Your Post is Live**:
   - GitHub Pages will automatically rebuild your site (takes 1-2 minutes)
   - Your new post will appear on the blog page

## File Structure

```
/
├── _config.yml          # Jekyll configuration
├── _layouts/            # Page templates
│   ├── default.html     # Main site layout
│   └── post.html        # Blog post layout
├── _posts/              # Blog posts go here
│   ├── 2024-01-15-understanding-ndis-support-coordination.html
│   ├── 2024-01-20-daily-living-skills-independence-at-home.html
│   └── 2024-01-25-community-participation-building-connections.html
├── css/                 # Stylesheets
├── img/                 # Images
├── js/                  # JavaScript files
├── blog.html            # Blog listing page
├── index.html           # Homepage
└── [other pages].html   # Your existing pages
```

## Writing Tips for Blog Posts

### Content Guidelines:
- **Length**: Aim for 800-2000 words for comprehensive posts
- **Structure**: Use headings (h2, h3) to break up content
- **Tone**: Professional but approachable, matching your brand
- **Topics**: Focus on disability support, NDIS information, health tips, community stories

### HTML Formatting:
- Use `<p>` tags for paragraphs
- Use `<h2>` and `<h3>` for headings
- Use `<strong>` for bold text
- Use `<em>` for italic text
- Use `<ul>` and `<li>` for bullet points when needed

### Categories to Use:
- "NDIS Support" - for NDIS-related content
- "Daily Living" - for independence and daily life skills
- "Community" - for community participation and social topics
- "Health Tips" - for health and wellness advice
- "News" - for company news and updates
- "Stories" - for participant stories and testimonials

## Adding Images to Blog Posts

1. **Upload Images**:
   - Add your images to the `img/` folder in your repository
   - Use descriptive filenames like `ndis-planning-guide.jpg`

2. **Reference in Posts**:
   - Set the `featured_image` in your post header: `featured_image: "img/your-image.jpg"`
   - Add images in content: `<img src="img/your-image.jpg" alt="Description" />`

## Customization Options

### Changing Colors/Styles:
- Edit the CSS files in the `css/` folder
- The main stylesheet is `css/skin.css`

### Adding New Pages:
- Create new HTML files in the root directory
- Add them to the navigation menu in `_layouts/default.html`

### Modifying the Blog Layout:
- Edit `_layouts/post.html` for individual post layout
- Edit `blog.html` for the blog listing page

## Troubleshooting

### Common Issues:

1. **Site not updating**:
   - Check the "Actions" tab in your GitHub repository for build errors
   - Ensure your post filename follows the correct format: `YYYY-MM-DD-title.html`

2. **Images not showing**:
   - Make sure image paths are correct: `img/filename.jpg`
   - Ensure images are uploaded to the `img/` folder

3. **Post not appearing**:
   - Check the date in your post - future dates won't show
   - Ensure the post is in the `_posts/` folder
   - Verify the filename format is correct

### Getting Help:
- Check GitHub Pages documentation: https://docs.github.com/en/pages
- Jekyll documentation: https://jekyllrb.com/docs/

## Maintenance

### Regular Tasks:
- **Daily**: Add new blog posts as needed
- **Weekly**: Review and respond to any build errors
- **Monthly**: Update any outdated information in existing posts

### Backup:
- Your content is automatically backed up on GitHub
- Consider downloading a copy of your repository periodically

## Advanced Features

### SEO Optimization:
- Each post automatically generates meta tags
- Use descriptive titles and excerpts
- Include relevant keywords naturally in your content

### Social Sharing:
- Posts include Open Graph meta tags for social media sharing
- Featured images will appear when shared on social platforms

### Analytics:
- You can add Google Analytics by editing `_layouts/default.html`
- Add the tracking code before the closing `</head>` tag

---

## Support

If you need help with your blog setup or have questions about adding content, refer to this guide or consult the GitHub Pages and Jekyll documentation linked above.

Your blog is now ready to help you share valuable content with your community while maintaining the professional look and feel of your Care By Nurse website.

