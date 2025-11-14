# Blogging Instructions for Your Website

This guide will help you create and publish blog posts on your website.

## Folder Structure

Your blog posts should be placed in the `blog/` folder. Each blog post should be a separate HTML file.

## Creating a New Blog Post

### Step 1: Create the HTML File

1. Create a new HTML file in the `blog/` folder (e.g., `blog/world-bank-data-visualization.html`)
2. Use the following template structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Blog Post Title - Research Portfolio</title>
    <link rel="stylesheet" href="../assets/styles.css">
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <a href="../index.html" class="logo">Research Portfolio</a>
                <nav>
                    <a href="../index.html">Home</a>
                    <a href="../page/publications.html">Publications</a>
                    <a href="../page/projects.html">Projects</a>
                    <a href="../page/about.html">About</a>
                    <a href="../page/contact.html">Contact</a>
                    <a href="../blog/index.html">Blog</a>
                </nav>
            </div>
        </div>
    </header>

    <main>
        <div class="container">
            <section class="hero">
                <h1>Your Blog Post Title</h1>
                <p>Subtitle or brief description</p>
            </section>

            <article class="section" style="max-width: 800px; margin: 0 auto;">
                <div style="color: rgba(255, 255, 255, 0.9); line-height: 1.8;">
                    <!-- Your blog content goes here -->
                    
                    <h2 style="color: #ffffff; margin-top: 2rem; margin-bottom: 1rem;">Section Title</h2>
                    <p style="margin-bottom: 1.5rem;">
                        Your paragraph text here.
                    </p>
                    
                    <!-- Add images/figures here -->
                    <figure style="margin: 2rem 0; text-align: center;">
                        <img src="../assets/images/your-image.png" alt="Description of image" 
                             style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);">
                        <figcaption style="margin-top: 0.5rem; font-size: 0.9rem; color: rgba(255, 255, 255, 0.7);">
                            Figure 1: Caption describing your figure
                        </figcaption>
                    </figure>
                    
                </div>
            </article>
        </div>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 Research Portfolio. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
```

### Step 2: Add Your Content

- Replace "Your Blog Post Title" with your actual title
- Write your content in the `<article>` section
- Use HTML tags for formatting:
  - `<h2>`, `<h3>` for headings
  - `<p>` for paragraphs
  - `<ul>`, `<ol>`, `<li>` for lists
  - `<strong>`, `<em>` for emphasis
  - `<a href="...">` for links
  - `<code>` for inline code

### Step 3: Add Figures/Images

1. **Create an images folder in assets:**
   - Create `assets/images/` folder if it doesn't exist
   - Place your images there

2. **Add images to your blog post:**
   ```html
   <figure style="margin: 2rem 0; text-align: center;">
       <img src="../assets/images/your-figure.png" 
            alt="Description of the figure" 
            style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);">
       <figcaption style="margin-top: 0.5rem; font-size: 0.9rem; color: rgba(255, 255, 255, 0.7);">
           Figure 1: Your figure caption here
       </figcaption>
   </figure>
   ```

3. **Image Guidelines:**
   - Use descriptive filenames (e.g., `world-bank-gdp-chart.png`)
   - Keep image file sizes reasonable (optimize if needed)
   - Use PNG, JPG, or SVG formats
   - Always include an `alt` attribute for accessibility
   - The path from blog posts is: `../assets/images/your-image.png`

### Step 4: Update the Blog Index Page

After creating your blog post, update `blog/index.html` to add a link to your new post:

```html
<a href="world-bank-data-visualization.html" class="link-card">
    <h3>World Bank Data Visualization</h3>
    <p style="margin-bottom: 0.5rem; color: rgba(255,255,255,0.85);">November 14, 2025</p>
    <p>Exploring global economic trends through data visualization of World Bank datasets.</p>
</a>
```

## Best Practices

1. **File Naming:** Use lowercase with hyphens (e.g., `world-bank-data-visualization.html`)
2. **Consistency:** Keep the same header and footer structure across all blog posts
3. **Styling:** Use inline styles for blog-specific formatting to maintain consistency with your site's design
4. **Images:** Always include captions for figures to provide context
5. **Links:** Use relative paths (e.g., `../assets/images/` from blog posts)
6. **Dates:** Include publication dates in your blog index entries

## Example Blog Post Structure

```html
<article class="section" style="max-width: 800px; margin: 0 auto;">
    <div style="color: rgba(255, 255, 255, 0.9); line-height: 1.8;">
        <!-- Introduction -->
        <p style="margin-bottom: 1.5rem;">
            Introduction paragraph...
        </p>
        
        <!-- Section 1 -->
        <h2 style="color: #ffffff; margin-top: 2rem; margin-bottom: 1rem;">Section 1 Title</h2>
        <p style="margin-bottom: 1.5rem;">
            Content...
        </p>
        
        <!-- Figure -->
        <figure style="margin: 2rem 0; text-align: center;">
            <img src="../assets/images/figure1.png" alt="Description" 
                 style="max-width: 100%; height: auto; border-radius: 10px; box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);">
            <figcaption style="margin-top: 0.5rem; font-size: 0.9rem; color: rgba(255, 255, 255, 0.7);">
                Figure 1: Caption
            </figcaption>
        </figure>
        
        <!-- Section 2 -->
        <h2 style="color: #ffffff; margin-top: 2rem; margin-bottom: 1rem;">Section 2 Title</h2>
        <p style="margin-bottom: 1.5rem;">
            More content...
        </p>
        
        <!-- Conclusion -->
        <h2 style="color: #ffffff; margin-top: 2rem; margin-bottom: 1rem;">Conclusion</h2>
        <p style="margin-bottom: 1.5rem;">
            Conclusion paragraph...
        </p>
    </div>
</article>
```

## Quick Checklist

- [ ] Created HTML file in `blog/` folder
- [ ] Added proper title and meta tags
- [ ] Wrote your content
- [ ] Added images to `assets/images/` folder
- [ ] Included image references with proper paths
- [ ] Added figure captions
- [ ] Updated `blog/index.html` with link to new post
- [ ] Tested all links and images

Happy blogging!

