# UC ERIC Lab Website

This is the official website for the UC ERIC Lab (Embodied and Responsible Interaction and Communication) at UCSC/UCSB.

## GitHub Pages Deployment

This website is now configured for automatic deployment to GitHub Pages using static HTML files.

### Quick Start

1. **Fork or clone this repository**
   ```bash
   git clone https://github.com/your-username/eric-lab-website.git
   cd eric-lab-website
   ```

2. **Enable GitHub Pages**
   - Go to your repository settings
   - Navigate to "Pages" in the sidebar
   - Under "Source", select "GitHub Actions"
   - The site will automatically deploy when you push to the main branch

3. **Your site will be available at:**
   ```
   https://your-username.github.io/eric-lab-website
   ```

### File Structure

```
├── index.html           # Home page (converted from Flask template)
├── people.html          # People page
├── publications.html    # Publications page
├── sponsors.html        # Sponsors page
├── contact.html         # Contact page
├── static/              # CSS, JS, and images
│   ├── css/
│   ├── js/
│   └── image/
└── .github/workflows/   # GitHub Actions for deployment
    └── deploy.yml
```

### Local Development

To test the site locally:

```bash
# Start a local web server
python3 -m http.server 8000

# Open your browser and go to:
# http://localhost:8000
```

### Making Updates

1. Edit the HTML files directly or modify the content
2. Test locally using the web server
3. Commit and push your changes:
   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```
4. GitHub Actions will automatically deploy your changes

### Migration from Flask

This site was originally a Flask application but has been converted to static HTML files for GitHub Pages deployment. The original Flask files are preserved in the repository but are excluded from deployment via `.gitignore`.

### Original Flask Version

For reference, the original Flask application files are still included:
- `init.py` - Flask application with routing
- `db.py` - Database functions  
- `app.wsgi` - WSGI configuration
- `requirements.txt` - Python dependencies
- `templates/` - Original Flask templates

These files are not used in the GitHub Pages deployment but are kept for historical reference.

## Contact

For questions about this website, please contact the ERIC Lab team or visit our [contact page](contact.html).