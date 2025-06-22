# 🎨 MarbaLabs Portfolio Website

A modern, responsive portfolio website showcasing MarbaLabs - a creative collective of artists, developers, and designers based in Marbella and London.

![MarbaLabs](static/logos/MARBALABS/Logo%20Files/For%20Web/png/Color%20logo%20-%20no%20background.png)

## 🌟 About MarbaLabs

MarbaLabs is a creative collective that bridges the gap between art, technology, and design. We specialize in blockchain development, NFT creation, gaming, and digital experiences, crafting solutions that push boundaries and create meaningful connections in the decentralized world.

## 🚀 Featured Projects

### 🐦 [Birb NFT](https://birb-nft.tech)
A unique NFT collection featuring adorable bird characters with rare traits and utilities. Built on cutting-edge blockchain technology with a focus on community and creativity.

### 🎮 [TonFlip](https://tonflip.bot)
An engaging gaming platform on the TON blockchain featuring coin flip mechanics and provably fair gameplay. Experience the thrill of decentralized gaming.

## 🛠️ Technology Stack

- **Framework**: [SvelteKit](https://kit.svelte.dev/) - Modern, fast, and lightweight
- **Styling**: CSS3 with modern features (Grid, Flexbox, Custom Properties)
- **Fonts**: [Inter](https://rsms.me/inter/) - Clean, modern typography
- **Build Tool**: [Vite](https://vitejs.dev/) - Lightning fast development
- **Package Manager**: npm

## ✨ Features

- 📱 **Responsive Design** - Works perfectly on all devices
- 🎭 **Modern UI/UX** - Clean, professional interface with smooth animations
- 🚀 **Fast Performance** - Optimized with SvelteKit and Vite
- 🎨 **Component-Based** - Modular architecture for easy maintenance
- 🔗 **Smooth Navigation** - Animated scrolling and fixed navbar
- 📧 **Contact Integration** - Direct email links
- 🌐 **SEO Optimized** - Proper meta tags and semantic HTML

## 🏁 Quick Start

### Prerequisites
- Node.js (16.0 or later)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/MarbaLabs_page.git
   cd MarbaLabs_page
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with hot reload |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build locally |
| `npm run check` | Run Svelte type checking |

## 📁 Project Structure

```
MarbaLabs_page/
├── src/
│   ├── lib/
│   │   └── components/
│   │       ├── Hero.svelte      # Hero section with logo and CTA
│   │       ├── Navbar.svelte    # Fixed navigation
│   │       ├── About.svelte     # About section
│   │       ├── Projects.svelte  # Project showcase cards
│   │       ├── Contact.svelte   # Contact section
│   │       └── Footer.svelte    # Footer component
│   ├── routes/
│   │   └── +page.svelte         # Main page
│   └── app.html                 # HTML template
├── static/
│   └── logos/                   # Company logos and assets
├── package.json
├── svelte.config.js
└── vite.config.js
```

## 🎨 Design Features

### Color Palette
- **Primary Orange**: `#ff8000` - MarbaLabs brand color
- **Gradient Backgrounds**: Modern gradient overlays
- **Project Colors**: 
  - Birb NFT: Blue gradient (`#4facfe` to `#00f2fe`)
  - TonFlip: Pink/Yellow gradient (`#fa709a` to `#fee140`)

### Typography
- **Font Family**: Inter - Clean, modern, and highly readable
- **Responsive Sizes**: Scales appropriately across all devices
- **Visual Hierarchy**: Clear distinction between headings and body text

### Animations
- Smooth scrolling navigation
- Hover effects on interactive elements
- Fade-in navbar on scroll
- Card hover animations

## 🚀 Deployment

The site can be deployed to various platforms:

### Vercel (Recommended)
```bash
npm i -g vercel
vercel
```

### Netlify
```bash
npm run build
# Upload dist/ folder to Netlify
```

### GitHub Pages
```bash
npm run build
# Deploy the build folder to gh-pages branch
```

## 📧 Contact

- **Email**: [marbalabs@gmail.com](mailto:marbalabs@gmail.com)
- **Locations**: Marbella, Spain & London, UK

## 🤝 Contributing

We welcome contributions! Please feel free to submit issues and enhancement requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

© 2024 Marba Labs. All rights reserved.

---

## 🔗 Links

- 🌐 **Live Site**: https://marbalabs.info
- 🐦 **Birb NFT**: [birb-nft.tech](https://birb-nft.tech)
- 🎮 **TonFlip**: [tonflip.bot](https://tonflip.bot)

---

*Built with ❤️ by MarbaLabs using SvelteKit*
