# GitHub Pages Deployment Instructions

## Quick Setup

1. **Create GitHub Repository**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: RAGHIM Widget Test"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/github_widget_test.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**:
   - Go to repository Settings
   - Scroll to "Pages" section
   - Source: "Deploy from a branch"
   - Branch: "main"
   - Folder: "/ (root)"
   - Click "Save"

3. **Access Your Test Page**:
   - URL: `https://YOUR_USERNAME.github.io/github_widget_test`
   - The widget should appear in the bottom-right corner

## Backend Configuration Required

Before the widget works, add your GitHub Pages domain to the RAGHIM backend:

```bash
# In your backend environment variables
ALLOWED_ORIGINS=http://34.65.50.3,http://localhost:8083,http://localhost:3002,https://YOUR_USERNAME.github.io
```

## Testing Checklist

- [ ] Repository created and files uploaded
- [ ] GitHub Pages enabled
- [ ] Backend ALLOWED_ORIGINS updated
- [ ] Test page loads successfully
- [ ] Widget appears in bottom-right corner
- [ ] Send button works
- [ ] Enter key works
- [ ] Messages are sent and received
- [ ] No CORS errors in browser console

## Troubleshooting

**Widget not appearing?**
- Check browser console for JavaScript errors
- Verify GitHub Pages is deployed successfully

**CORS errors?**
- Ensure GitHub Pages domain is in backend ALLOWED_ORIGINS
- Check backend logs for blocked requests

**Messages not sending?**
- Verify RAGHIM server is running
- Check network tab for failed API calls
- Ensure embed token is correct
