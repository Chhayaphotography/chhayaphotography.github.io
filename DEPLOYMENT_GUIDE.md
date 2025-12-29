# Chhaya Photography - Deployment Guide

## ✅ Website Ready for Deployment

Your website has been successfully prepared with:
- **New maroon/red color scheme** matching your logo (#8B1538, #C41E3A, #D32F2F)
- **All image paths fixed** for proper loading
- **Complete directory structure** ready for web hosting
- **Optimized performance** with lazy loading and smooth scrolling

---

## 📁 Directory Structure

```
D:\For_chhaya_photography\     ← Upload this entire folder
├── index.html                  ← Homepage (57.8 KB)
├── gallery.html                ← Full portfolio gallery (23.1 KB)
├── about/                      ← About Us page
├── contact/                    ← Contact page
├── gallery/                    ← Gallery page (old)
├── css/                        ← Custom styles
│   └── custom.css
├── js/                         ← JavaScript files
│   └── main.js
├── wp-content/                 ← All images and media
│   └── uploads/
│       ├── 2023/11/            ← Logo and older images
│       ├── 2024/03/            ← Portfolio images
│       └── 2024/06/            ← Recent photos
├── fonts/                      ← Font files
└── backup_old_site/            ← Old WordPress files (DO NOT upload)
```

---

## 🚀 How to Deploy

### Option 1: FTP Upload (Most Common)

1. **Get FTP credentials** from your hosting provider:
   - FTP Host (e.g., ftp.yourdomain.com)
   - Username
   - Password
   - Port (usually 21)

2. **Use an FTP client** like FileZilla (free):
   - Download: https://filezilla-project.org/

3. **Upload all files EXCEPT `backup_old_site/`**:
   ```
   Upload these folders/files to your web root (usually public_html/ or www/):
   ✅ index.html
   ✅ gallery.html
   ✅ about/
   ✅ contact/
   ✅ gallery/
   ✅ css/
   ✅ js/
   ✅ wp-content/
   ✅ fonts/
   
   ❌ DO NOT upload: backup_old_site/ (it's just for backup)
   ```

4. **Verify** by visiting your domain (e.g., https://chhayaphotography.com)

---

### Option 2: cPanel File Manager

1. Log into your hosting **cPanel**
2. Open **File Manager**
3. Navigate to `public_html/` (or `www/`)
4. **Delete old WordPress files** (if any) - MAKE A BACKUP FIRST!
5. **Upload** all files/folders listed above (except backup_old_site/)
6. Visit your website

---

### Option 3: Direct Server Access (SSH/SFTP)

If you have SSH access:

```bash
# Upload via SCP/SFTP to your server
scp -r D:\For_chhaya_photography/* username@yourserver.com:/path/to/public_html/

# Or use rsync (excludes backup)
rsync -avz --exclude 'backup_old_site' D:\For_chhaya_photography/* username@yourserver.com:/path/to/public_html/
```

---

## ✨ What's New in This Version

### 🎨 **Brand Colors Updated**
- Changed from amber/orange (#d97706) to maroon/red (#8B1538) to match your logo
- All buttons, links, and accents now use your brand colors
- Consistent color scheme across all pages

### 📸 **Image Loading Fixed**
- All gallery images now load correctly
- Paths updated from `../wp-content/` to `wp-content/`
- All photos accessible in same directory structure

### 🏗️ **Directory Structure Simplified**
- No more nested `/modern/` folder
- Direct deployment from root directory
- Clean, professional structure for web hosting

### ⚡ **Performance Optimized**
- Lazy loading for images
- Throttled scroll events for smooth performance
- GPU-accelerated animations
- Optimized for fast load times

---

## 🌐 Website Features

### **Complete Nepali Wedding Package**
- Photography Services
- Videography Services (featuring IMDB cinematographer Rameshwar Karki)
- Wedding Decorations
- Wedding Maalaa (Traditional Garlands)

### **SEO Optimized**
- Keywords: Nepali wedding photography, Indian wedding photography, cultural weddings
- Meta descriptions for all pages
- Proper heading structure

### **Modern Design**
- Responsive mobile-first design
- Smooth scroll animations (AOS)
- Modern font pairing (Playfair Display + Inter)
- Professional Tailwind CSS styling

---

## 📋 Pre-Launch Checklist

Before going live, verify:

- [ ] All pages load correctly (index.html, gallery.html, about/, contact/)
- [ ] Images appear properly in gallery
- [ ] Navigation links work between pages
- [ ] Contact form functions (if backend is set up)
- [ ] Mobile responsive design works on phone/tablet
- [ ] Logo appears in header
- [ ] New maroon/red color scheme is visible
- [ ] Social media links work (if added)
- [ ] Domain SSL certificate is active (https://)

---

## 🆘 Troubleshooting

### Images Not Loading?
- Check that `wp-content/` folder is in the same directory as `index.html`
- Verify file permissions (folders: 755, files: 644)

### Pages Showing 404 Error?
- Ensure all folders uploaded correctly
- Check that `index.html` is in the root directory
- Some servers need `index.html` renamed to `index.htm` or `default.html`

### Colors Still Look Orange?
- Hard refresh your browser: `Ctrl + Shift + R` (Windows) or `Cmd + Shift + R` (Mac)
- Clear browser cache
- Try in incognito/private browsing mode

---

## 📞 Support

If you need help with:
- Domain setup
- Email configuration
- Contact form backend
- SSL certificate
- Server configuration

Contact your web hosting provider's support team.

---

## 🎉 Your Website is Ready!

Your modern, optimized photography website is ready to showcase your work to the world. The new color scheme matches your brand perfectly, and all images are properly configured.

**Upload the files and your beautiful website will be live!** 🚀

---

*Last Updated: December 29, 2024*
