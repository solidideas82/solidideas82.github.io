# Deployment Guide - GitHub Pages

## 🚀 Deploy Your Website to GitHub Pages

Follow these steps to make your website live on the internet:

### Step 1: Enable GitHub Pages

1. **Go to your repository:**
   Navigate to: https://github.com/solidideas82/solidideasaero-web

2. **Open Settings:**
   - Click the **"Settings"** tab (top right of your repository)

3. **Find Pages settings:**
   - In the left sidebar, scroll down and click **"Pages"

4. **Configure the source:**
   - Under **"Build and deployment"**
   - Under **"Source"**, select **"Deploy from a branch"**
   - Under **"Branch"**, select **"main"** from the dropdown
   - Select **"/ (root)"** as the folder
   - Click **"Save"**

5. **Wait for deployment:**
   - GitHub will start building your site (takes 1-2 minutes)
   - Refresh the page after a minute

6. **Get your live URL:**
   - Your site will be live at:
   ```
   https://solidideas82.github.io/solidideasaero-web/
   ```

### Step 2: Verify Your Deployment

Once deployed, test your website:
- ✅ Check all navigation links work
- ✅ Verify images load correctly
- ✅ Test on mobile devices
- ✅ Confirm contact information is correct

### Step 3: Custom Domain (Optional)

If you want to use a custom domain like `www.solidideasaero.com`:

1. **Purchase a domain** from a registrar (GoDaddy, Namecheap, etc.)

2. **Create a CNAME file** in your repository:
   ```
   www.solidideasaero.com
   ```

3. **Configure DNS settings** at your domain registrar:
   - Add a CNAME record pointing to: `solidideas82.github.io`
   - Or add A records pointing to GitHub's IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```

4. **Enable custom domain in GitHub Pages settings**

5. **Enable HTTPS** (recommended)

### Common Issues & Solutions

**Issue: 404 Error**
- Solution: Make sure `index.html` is in the root directory
- Check that GitHub Pages is enabled on the `main` branch

**Issue: Images not loading**
- Solution: Verify image filenames match exactly (case-sensitive)
- Check that images are committed to the repository

**Issue: Changes not showing**
- Solution: Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Wait a few minutes for GitHub to rebuild

**Issue: Styles not applying**
- Solution: Verify `style.css` is in the same directory as `index.html`
- Check for typos in the `<link>` tag

### Update Your Website

To make changes after deployment:

1. **Edit files directly on GitHub:**
   - Click on the file you want to edit
   - Click the pencil icon (Edit)
   - Make your changes
   - Commit changes

2. **Or use Git locally:**
   ```bash
   git clone https://github.com/solidideas82/solidideasaero-web.git
   cd solidideasaero-web
   # Make your edits
   git add .
   git commit -m "Update website content"
   git push origin main
   ```

3. **GitHub will automatically rebuild** (takes 1-2 minutes)

### Performance Tips

- Optimize images before uploading
- Keep file sizes under 500KB for images
- Use compressed CSS/JS if needed
- Enable browser caching

### Security & Monitoring

- ✅ Enable HTTPS (automatic with GitHub Pages)
- ✅ Use `robots.txt` for SEO control
- ✅ Monitor with Google Search Console
- ✅ Set up Google Analytics (optional)

---

## 📞 Need Help?

If you encounter issues:
- Check [GitHub Pages documentation](https://docs.github.com/en/pages)
- Contact: Andres@solidideasaero.com

**Your site is now ready to go live!** 🎉