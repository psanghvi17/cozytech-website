# CozyTech Website

Welcome to the CozyTech website! This is a modern, responsive website for CozyTech with the tagline "We make tech cozy."

## 🌐 Live Site

The website is hosted at: **https://cozytech.co.in**

## 🚀 Features

- **Modern Design**: Clean, beautiful interface with smooth animations
- **Fully Responsive**: Works perfectly on desktop, tablet, and mobile devices
- **Fast Loading**: Optimized for performance
- **Smooth Scrolling**: Enhanced user experience with smooth navigation
- **Interactive Elements**: Engaging animations and hover effects

## 📁 Project Structure

```
cozytech-website/
├── index.html      # Main HTML file
├── styles.css      # All styling and responsive design
├── script.js       # JavaScript for interactivity
└── README.md       # This file
```

## 🛠️ Setup for GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `cozytech-website` (or any name you prefer)
3. Make it public (required for free GitHub Pages)
4. Don't initialize with README, .gitignore, or license

### Step 2: Push Your Code

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit your files
git commit -m "Initial commit: CozyTech website"

# Add your GitHub repository as remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/cozytech-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** section (in the left sidebar)
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**

### Step 4: Configure Custom Domain (cozytech.co.in)

1. In the same **Pages** settings, scroll to **Custom domain**
2. Enter `cozytech.co.in` and click **Save**
3. GitHub will create a `CNAME` file automatically

### Step 5: Configure DNS

You need to configure your DNS settings with your domain registrar:

1. Add a **CNAME** record:
   - **Type**: CNAME
   - **Name**: @ (or leave blank for root domain)
   - **Value**: `YOUR_USERNAME.github.io`
   - **TTL**: 3600 (or default)

2. Alternatively, if your registrar doesn't support CNAME for root domain, use **A records**:
   - **Type**: A
   - **Name**: @
   - **Value**: (Use GitHub Pages IP addresses - check current IPs from GitHub documentation)
   - Common IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`

3. For www subdomain, add:
   - **Type**: CNAME
   - **Name**: www
   - **Value**: `YOUR_USERNAME.github.io`

### Step 6: Wait for DNS Propagation

- DNS changes can take anywhere from a few minutes to 48 hours
- You can check propagation status using tools like [whatsmydns.net](https://www.whatsmydns.net)

### Step 7: Verify HTTPS

- GitHub Pages automatically provides SSL certificates via Let's Encrypt
- Once DNS is configured, HTTPS will be enabled automatically
- This may take a few hours after DNS propagation

## 🔧 Local Development

To view the website locally:

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/cozytech-website.git
cd cozytech-website
```

2. Open `index.html` in your web browser, or use a local server:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

3. Visit `http://localhost:8000` in your browser

## 📝 Customization

### Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #8b5cf6;
    --accent-color: #ec4899;
    /* ... */
}
```

### Content

- Edit `index.html` to change text content
- Modify sections, add new sections, or update existing ones
- Update contact information in the contact section

### Styling

- All styles are in `styles.css`
- The design is fully responsive with mobile-first approach
- Animations and transitions can be adjusted in the CSS file

## 🎨 Design Features

- **Gradient Backgrounds**: Beautiful animated gradient orbs
- **Smooth Animations**: Fade-in effects and hover transitions
- **Modern Typography**: Inter font family for clean readability
- **Card-based Layout**: Clean, organized content presentation
- **Interactive Navigation**: Smooth scrolling and active link highlighting

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 License

This website is proprietary to CozyTech.

## 🤝 Support

For issues or questions, please contact: hello@cozytech.co.in

---

**CozyTech** - We make tech cozy ✨
