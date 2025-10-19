# RAGHIM Widget Test - GitHub Pages

This repository contains a test page for the RAGHIM AI Chat Widget deployed on GitHub Pages.

## 🚀 Live Demo

Visit the live test page: `https://yourusername.github.io/github_widget_test`

## 📋 What This Tests

- ✅ Widget embedding on external websites
- ✅ CORS handling from GitHub Pages domain
- ✅ API communication with RAGHIM backend
- ✅ Widget functionality (chat, minimize, close)
- ✅ Cross-origin security

## 🔧 Configuration

### Widget Details
- **Name**: test_widget1
- **API Endpoint**: http://34.65.50.3:8006/api/chat/widget/
- **Embed Token**: qIMqOHjlj6ZU7KBY2yQCR7Z_xErC6bsqeE153nuy9Es
- **Widget ID**: bcb16eae-b483-4447-98de-707efed8116f

### Backend Requirements
The RAGHIM backend needs to include GitHub Pages domain in `ALLOWED_ORIGINS`:
```bash
ALLOWED_ORIGINS=http://34.65.50.3,http://localhost:8083,http://localhost:3002,https://yourusername.github.io
```

## 🧪 Testing Instructions

1. **Deploy to GitHub Pages**:
   - Create a new repository
   - Upload these files
   - Enable GitHub Pages in repository settings

2. **Test the Widget**:
   - Visit your GitHub Pages URL
   - Look for the chat widget in bottom-right corner
   - Try sending messages like "Hello" or "What is RAG?"
   - Check browser console (F12) for any errors

3. **Verify Functionality**:
   - ✅ Widget loads and displays
   - ✅ Send button works
   - ✅ Enter key works
   - ✅ Messages are sent and received
   - ✅ Minimize/close buttons work
   - ✅ No CORS errors in console

## 📁 Files

- `index.html` - Main test page with embedded widget
- `README.md` - This documentation

## 🔍 Troubleshooting

### Common Issues

1. **CORS Errors**: Make sure GitHub Pages domain is in backend `ALLOWED_ORIGINS`
2. **Widget Not Loading**: Check browser console for JavaScript errors
3. **API Connection Failed**: Verify RAGHIM server is running and accessible
4. **Messages Not Sending**: Check network tab for failed requests

### Debug Steps

1. Open browser Developer Tools (F12)
2. Check Console tab for errors
3. Check Network tab for failed requests
4. Verify widget initialization logs

## 📞 Support

If you encounter issues:
1. Check the browser console for error messages
2. Verify the RAGHIM backend is running
3. Ensure GitHub Pages domain is whitelisted in backend
4. Test with a simple "Hello" message first

---

**Powered by RAGHIM AI** 🤖
