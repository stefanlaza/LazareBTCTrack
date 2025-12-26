# 🪙 Lazare Bitcoin Address Tracker

A beautiful, minimalist Bitcoin address tracker with real-time data from Mempool.space. Built with glassmorphism design and ultra-lightweight architecture.

![Lazare Bitcoin Tracker](https://img.shields.io/badge/Bitcoin-Tracker-orange)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)


## ✨ Features

- 🔍 **Real-time tracking** - Live Bitcoin address data from Mempool.space
- 📊 **Balance overview** - View balance, total received, and total sent
- 📜 **Transaction history** - See recent transactions with detailed information
- 🔄 **Compare mode** - Compare up to 2 addresses side-by-side
- 🎨 **Glassmorphism UI** - Modern, elegant design with dark theme
- 📱 **Fully responsive** - Works perfectly on mobile, tablet, and desktop
- ⚡ **Lightning fast** - Pure HTML/CSS/JS, no build process required
- 🐳 **Docker ready** - Deploy anywhere in seconds

## 🚀 Quick Start

### Option 1: Open Locally (Instant)

Simply open `index.html` in your browser. That's it!

### Option 2: Python Server (Simple)
```bash
python3 -m http.server 8080
```

Visit: `http://localhost:8080`

### Option 3: Docker (Recommended)
```bash
# Build the image
docker build -t lazare-btc .

# Run the container
docker run -d -p 8080:80 --name lazare-btc lazare-btc
```

Visit: `http://localhost:8080`

**Or use Docker Compose:**
```bash
docker-compose up -d
```

## 📦 Deployment

### Deploy to Netlify (Easiest - Free)

1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag and drop `index.html`
3. Done! Your site is live with HTTPS

### Deploy to GitHub Pages (Free)
```bash
# Initialize git repository
git init
git add .
git commit -m "Initial commit"
git branch -M main

# Push to GitHub (create repo first at github.com/new)
git remote add origin https://github.com/YOUR_USERNAME/lazare-bitcoin-tracker.git
git push -u origin main

# Enable GitHub Pages in repository settings
```

Your site will be live at: `https://YOUR_USERNAME.github.io/lazare-bitcoin-tracker/`

### Deploy to AWS S3 (Scalable - ~$1/month)
```bash
# Create S3 bucket
aws s3 mb s3://lazare-bitcoin-tracker

# Upload file
aws s3 cp index.html s3://lazare-bitcoin-tracker/index.html --acl public-read

# Enable static website hosting
aws s3 website s3://lazare-bitcoin-tracker/ --index-document index.html
```

## 🎯 Usage

1. **Track a single address:**
   - Enter a Bitcoin address in the search bar
   - Click "Track Address"
   - View balance, transactions, and statistics

2. **Compare addresses:**
   - Click "Compare Addresses" button
   - Add your first address
   - Add a second address
   - View side-by-side comparison

3. **Track another address:**
   - Click "Track Another Address" to clear and start over

## 🛠️ Tech Stack

- **HTML5** - Structure
- **Tailwind CSS** - Styling (via CDN)
- **Vanilla JavaScript** - Logic
- **Lucide Icons** - Beautiful icons
- **Mempool.space API** - Bitcoin data source
- **Nginx Alpine** - Docker web server (2MB!)

## 📱 Supported Address Types

- ✅ Legacy (P2PKH): `1...`
- ✅ SegWit (P2SH): `3...`
- ✅ Native SegWit (Bech32): `bc1q...`
- ✅ Taproot (Bech32m): `bc1p...`

## 🎨 Design Features

- Dark gradient background (black to gray)
- Glassmorphism effects with backdrop blur
- Orange accents for Bitcoin branding
- Smooth animations and transitions
- Responsive grid layout
- Custom glass scrollbars

## 📝 File Structure
```
lazare-bitcoin-tracker/
├── index.html           # Main application file
├── Dockerfile           # Docker configuration
├── docker-compose.yml   # Docker Compose setup
├── README.md           # Documentation
└── .gitignore          # Git ignore rules
```

## 🐳 Docker Details

**Image:** nginx:alpine  
**Size:** ~2MB  
**Port:** 80 (maps to 8080 on host)  
**Base:** Alpine Linux

### Docker Commands
```bash
# Build
docker build -t lazare-btc .

# Run
docker run -d -p 8080:80 --name lazare-btc lazare-btc

# Stop
docker stop lazare-btc

# Remove
docker rm lazare-btc

# View logs
docker logs lazare-btc

# Using Docker Compose
docker-compose up -d      # Start
docker-compose down       # Stop
docker-compose logs -f    # View logs
```

## 🔧 Configuration

No configuration needed! The app uses Mempool.space's public API which requires no API key.

## 🌐 API Information

**Data Source:** [Mempool.space API](https://mempool.space/docs/api)  
**Rate Limits:** Reasonable use (no hard limits for public API)  
**Data:** Real-time blockchain data  
**No API Key Required**

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request


## 🙏 Acknowledgments

- [Mempool.space](https://mempool.space) for the excellent Bitcoin API
- [Tailwind CSS](https://tailwindcss.com) for utility-first CSS
- [Lucide Icons](https://lucide.dev) for beautiful icons

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](../../issues) page
2. Create a new issue with details
3. Include browser console errors if applicable


---

**Made with ❤️ for the Bitcoin community**
