# Behind The Science - Setup Instructions

## Welcome to Behind The Science! 🚀⚛️🛡️

You've successfully downloaded a complete science blogging website focused on India's Space, Nuclear, and Defence programs. This is a fully functional, professional website ready to run on your local computer.

## What's Included

**Your blog features:**
- ✅ Homepage with three featured articles
- ✅ Detailed articles on:
  - ISRO: India's Journey to the Stars
  - India's Nuclear Power: From Pokhran to Energy Independence
  - Made in India: Indigenous Defence Technology
- ✅ About page explaining the blog's mission
- ✅ Dark theme design with cyan/blue colors matching your logo
- ✅ Your custom "Behind The Science" logo integrated
- ✅ Fully responsive (works on mobile, tablet, desktop)
- ✅ Professional science/tech aesthetic

## File Structure

```
my-blog/
├── index.html          # Homepage with article previews
├── about.html          # About Behind The Science
├── css/
│   └── style.css       # Dark theme with cyan styling
├── images/
│   └── logo.jpg        # Your BTS logo
├── posts/
│   ├── isro.html       # ISRO space program article
│   ├── nuclear.html    # Nuclear program article
│   └── defence.html    # Defence program article
└── README.md           # This file
```

## 🚀 How to Run Your Blog Locally

### Method 1: Using Python (EASIEST - RECOMMENDED)

**Step-by-step instructions:**

1. **Extract the folder**:
   - Save the `my-blog` folder to your computer (e.g., Downloads or Desktop)

2. **Open Command Prompt/Terminal**:
   - **Windows**: Press `Win + R`, type `cmd`, press Enter
   - **Mac**: Press `Cmd + Space`, type `terminal`, press Enter
   - **Linux**: Press `Ctrl + Alt + T`

3. **Navigate to your folder**:
   ```bash
   cd C:\Users\BARC\Downloads\my-blog
   ```
   (Replace with your actual path)

4. **Start the server**:
   ```bash
   python -m http.server 8000
   ```
   
   If you get an error, try:
   ```bash
   python3 -m http.server 8000
   ```

5. **Open your browser**:
   - Go to: `http://localhost:8000`
   - Your blog should now be running!

6. **To stop the server**:
   - Press `Ctrl + C` in the terminal

### Method 2: Using VS Code Live Server

1. Open VS Code
2. Install the "Live Server" extension by Ritwick Dey
3. Open the `my-blog` folder in VS Code (File → Open Folder)
4. Right-click on `index.html`
5. Select "Open with Live Server"
6. Your blog opens automatically!

**Advantage**: Automatically refreshes when you edit files!

### Method 3: Using Node.js

If you have Node.js installed:

```bash
npm install -g http-server
cd path/to/my-blog
http-server
```

Then open: `http://localhost:8080`

## 🔧 Troubleshooting Common Issues

### Problem: "Python is not recognized"

**Solution**: Install Python
1. Go to https://www.python.org/downloads/
2. Download and install Python
3. ⚠️ IMPORTANT: Check "Add Python to PATH" during installation
4. Restart your terminal and try again

### Problem: CSS not loading (page looks plain/white)

**This was your exact issue! Here's how to fix it:**

1. **Make sure you're in the correct folder**:
   ```bash
   # First, navigate to the folder
   cd C:\Users\BARC\Downloads\my-blog
   
   # Then verify you're in the right place
   dir  (Windows) or ls (Mac/Linux)
   
   # You should see: index.html, css, images, posts folders
   ```

2. **Verify folder structure**:
   ```
   my-blog/
   ├── index.html
   ├── css/
   │   └── style.css    ← This file must exist!
   └── images/
       └── logo.jpg     ← Your logo must be here!
   ```

3. **Use a local server (not double-clicking the HTML)**:
   - DON'T just double-click index.html
   - DO run the Python server command first

4. **Check the correct URL**:
   - Use: `http://localhost:8000` ✅
   - NOT: `file:///C:/Users/...` ❌

### Problem: Logo not showing

Make sure `logo.jpg` is in the `images` folder inside `my-blog`.

### Problem: Links not working

Always access via `http://localhost:8000`, not by double-clicking the HTML file.

## 🎨 Customizing Your Blog

### Change Colors

Edit `css/style.css` and find these color codes:

```css
/* Main cyan/blue colors (matching your logo) */
#00d9ff  /* Bright cyan */
#00ff88  /* Green accent */

/* Background colors */
#0a0e27  /* Dark navy */
#1a1d3a  /* Slightly lighter navy */
```

You can use a color picker like https://htmlcolorcodes.com/ to find new colors.

### Add Your Social Media Links

In all HTML files, find the footer section:

```html
<div class="social-links">
    <a href="YOUR_YOUTUBE_URL">YouTube</a>
    <a href="YOUR_TWITTER_URL">Twitter</a>
    <a href="YOUR_INSTAGRAM_URL">Instagram</a>
</div>
```

Replace `#` with your actual social media URLs.

### Change Site Name or Tagline

In each HTML file, find:

```html
<h1 class="site-title">Behind The Science</h1>
<p class="site-tagline">Exploring India's Scientific Excellence</p>
```

Edit these to your liking!

### Add More Articles

1. Copy one of the existing post files (e.g., `isro.html`)
2. Rename it (e.g., `robotics.html`)
3. Edit the content inside
4. Add a new card in `index.html`:

```html
<article class="post-card">
    <div class="post-image space-bg">
        <div class="post-category">Your Category</div>
    </div>
    <div class="post-content">
        <span class="post-date">🗓️ February 5, 2026</span>
        <h2 class="post-title">
            <a href="posts/your-new-post.html">Your New Article Title</a>
        </h2>
        <p class="post-excerpt">
            Your article preview text here...
        </p>
        <a href="posts/your-new-post.html" class="read-more">Read More →</a>
    </div>
</article>
```

### Change Background Images

In `css/style.css`, find the post backgrounds:

```css
.space-bg { /* For space-related posts */ }
.nuclear-bg { /* For nuclear posts */ }
.defence-bg { /* For defence posts */ }
```

You can modify these or add new ones!

## 📱 Mobile Responsiveness

Your blog automatically adapts to different screen sizes:
- Desktop: Full layout with sidebar navigation
- Tablet: Adjusted spacing and font sizes
- Mobile: Stacked layout, optimized for touch

Test by resizing your browser window!

## 🌐 Publishing Your Blog Online (Optional)

Once you're happy with your blog locally, you can publish it online for free using:

1. **GitHub Pages** (Recommended)
   - Free hosting
   - Custom domain support
   - Tutorial: https://pages.github.com/

2. **Netlify**
   - Free tier available
   - Automatic deployments
   - Tutorial: https://www.netlify.com/

3. **Vercel**
   - Free hosting
   - Great performance
   - Tutorial: https://vercel.com/

## 💡 Tips for Success

1. **Keep Content Updated**: Regularly add new articles about recent developments
2. **Backup Your Work**: Save copies of your blog folder regularly
3. **Test After Changes**: Always check how the blog looks after editing
4. **Use Browser DevTools**: Press F12 to inspect and debug
5. **Learn HTML/CSS**: This will help you customize further

## 📚 Learning Resources

Want to enhance your blog? Learn more:
- **HTML/CSS**: https://www.w3schools.com/
- **Web Design**: https://developer.mozilla.org/
- **Color Schemes**: https://coolors.co/
- **Icons**: https://fontawesome.com/

## ❓ Need Help?

**Common mistakes to avoid:**
1. Not being in the correct folder when starting server
2. Missing the `css` or `images` folders
3. Trying to open HTML files directly instead of using a server
4. Forgetting to keep the terminal window open while viewing the blog

**Quick checklist if something doesn't work:**
- [ ] Am I in the `my-blog` folder in terminal?
- [ ] Did I start the Python server?
- [ ] Am I using `http://localhost:8000` in my browser?
- [ ] Are all files in the correct folders?

## 🎉 You're All Set!

Your "Behind The Science" blog is ready to go! Start the server, explore your blog, and begin customizing it to make it truly yours.

**Next steps:**
1. Run the local server
2. View your blog at `http://localhost:8000`
3. Read through the existing articles
4. Start planning your own content
5. Customize the design to your taste

Happy blogging about India's amazing scientific achievements! 🇮🇳🔬🚀

---

**Behind The Science** - Uncovering India's Scientific Excellence
