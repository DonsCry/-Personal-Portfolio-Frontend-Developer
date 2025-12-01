![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white)


<!-- QUALITY -->
![Responsive](https://img.shields.io/badge/Responsive-Yes-00b894?style=flat)
![Dashboard](https://img.shields.io/badge/UI-Dashboard-0984e3?style=flat)
![Charts](https://img.shields.io/badge/Charts-Enabled-6c5ce7?style=flat)

<!-- STATUS -->
![Version](https://img.shields.io/badge/version-1.0.0-blue?style=flat)
![Status](https://img.shields.io/badge/Status-Production_Ready-brightgreen?style=flat)
![Last Update](https://img.shields.io/badge/Updated-Active-success?style=flat)

<!-- LICENSE -->
![License](https://img.shields.io/badge/License-MIT-yellow?style=flat)

[![GitHub last commit](https://img.shields.io/github/last-commit/DonsCry/techflow-platform)](https://github.com/DonsCry/techflow-platform)
[![Lighthouse](https://img.shields.io/badge/Lighthouse-95%2B-brightgreen)](https://developers.google.com/web/tools/lighthouse)
[![Responsive](https://img.shields.io/badge/Responsive-Mobile%20Ready-blue)]()
![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Status](https://img.shields.io/badge/status-Production%20Ready-success)
# High-End Professional Portfolio Website

A modern, responsive portfolio website built with Next.js, Tailwind CSS, and Framer Motion. Designed to showcase frontend development projects and skills with a clean, professional aesthetic.

## 🎯 Features

### 1. **Hero Section**
- Professional headline: "Frontend UI Developer"
- Minimalist avatar with gradient border
- Call-to-action buttons (Hire Me + GitHub)
- Social media links (GitHub, LinkedIn, Email)
- Subtle scroll indicator animation

### 2. **Project Showcase**
- 6 featured projects in a responsive grid (1-3 columns)
- Each project includes:
  - Project thumbnail/emoji icon
  - Short description
  - Role/position
  - Technology stack badges
  - Demo and GitHub links
  - Hover animations

### 3. **Skills Section**
- Organized by categories:
  - Frontend (React, Next.js, TypeScript, Tailwind CSS)
  - UI/UX (Figma, Responsive Design, Animation, Accessibility)
  - Tools (Git, VS Code, Webpack, Docker)
  - Soft Skills (Problem Solving, Communication, etc.)
- Clean list layout with accent dots
- Hover effects on skill cards

### 4. **Contact Section**
- Contact information display:
  - Email
  - WhatsApp link
  - GitHub profile
  - LinkedIn profile
- Contact form with fields:
  - Name
  - Email
  - Message
- Form validation and submission handling

### 5. **Navigation & Footer**
- Sticky navbar with smooth animations
- Mobile-responsive hamburger menu
- Footer with quick links and social connections
- Copyright information

## 🛠️ Tech Stack

- **Framework**: Next.js 14
- **Styling**: Tailwind CSS 3
- **Animations**: Framer Motion 10
- **Icons**: Lucide React
- **Language**: TypeScript
- **Package Manager**: npm

## 📦 Installation

1. **Clone or navigate to the project directory**
```bash
cd portofolio-me
```

2. **Install dependencies**
```bash
npm install
```

3. **Run development server**
```bash
npm run dev
```

4. **Open in browser**
Navigate to `http://localhost:3000`

## 🚀 Build & Deploy

### Build for production
```bash
npm run build
npm start
```

### Deploy to Vercel (Recommended)
1. Push your code to GitHub
2. Import project in Vercel
3. Deploy with one click

### Deploy to Netlify
1. Connect your GitHub repository
2. Set build command: `npm run build`
3. Set publish directory: `.next`

## 📝 Customization

### Update Personal Information
Edit the following files to add your information:

**`app/layout.tsx`** - Update metadata
```typescript
export const metadata: Metadata = {
  title: 'Your Name - Portfolio',
  description: 'Your description here',
}
```

**`components/Hero.tsx`** - Update social links
```typescript
href="https://github.com/yourprofile"
href="mailto:your@email.com"
```

**`components/Projects.tsx`** - Add your projects
```typescript
const projects = [
  {
    id: 1,
    title: 'Your Project',
    description: 'Project description',
    role: 'Your role',
    tech: ['React', 'Tailwind'],
    image: '🎨',
    demo: 'https://demo-link.com',
    github: 'https://github.com/yourrepo',
  },
  // Add more projects...
]
```

**`components/Skills.tsx`** - Update your skills
```typescript
const skills = [
  { category: 'Frontend', items: ['React', 'Next.js', 'Your Skills'] },
  // Add more categories...
]
```

**`components/Contact.tsx`** - Update contact information
```typescript
href="revalsaputra350@gmail.com"
href="https://wa.me/62+81936514430"
```

## 🎨 Design System

### Color Scheme
- **Dark Background**: `#0a0a0a`
- **Secondary Dark**: `#1a1a1a`
- **Tertiary Dark**: `#2d2d2d`
- **Accent Color**: `#00d9ff` (Cyan)
- **Secondary Accent**: Blue gradient

### Typography
- **Font Family**: System fonts (Apple System, Segoe UI, etc.)
- **Headings**: Bold, gradient text for emphasis
- **Body**: Regular weight, gray-400 for secondary text

### Spacing & Layout
- **Max Width**: 7xl (80rem)
- **Padding**: Responsive (4px to 8px)
- **Gap**: 6px to 12px between elements
- **Border Radius**: 8px for cards

## 🎬 Animation Details

- **Page Load**: Staggered fade-in animations
- **Navbar**: Slide down from top
- **Sections**: Fade in on scroll (whileInView)
- **Cards**: Lift up on hover with smooth transitions
- **Buttons**: Scale on hover and tap
- **Scroll Indicator**: Continuous up-down animation

## 📱 Responsive Design

- **Mobile**: Single column layout, hamburger menu
- **Tablet**: 2-column grid for projects
- **Desktop**: 3-column grid for projects, full navigation

## 🔍 SEO Optimization

- Semantic HTML structure
- Meta tags for title and description
- Proper heading hierarchy
- Alt text for images
- Open Graph ready

## 📄 File Structure

```
portofolio-me/
├── app/
│   ├── layout.tsx          # Root layout
│   ├── page.tsx            # Home page
│   └── globals.css         # Global styles
├── components/
│   ├── Navbar.tsx          # Navigation bar
│   ├── Hero.tsx            # Hero section
│   ├── Projects.tsx        # Projects showcase
│   ├── Skills.tsx          # Skills section
│   ├── Contact.tsx         # Contact section
│   └── Footer.tsx          # Footer
├── package.json            # Dependencies
├── tailwind.config.js      # Tailwind configuration
├── tsconfig.json           # TypeScript configuration
└── README.md               # This file
```

## 🤝 Contributing

Feel free to fork this project and customize it for your own portfolio!

## 📄 License

This project is open source and available under the MIT License.

## 💡 Tips for Best Results

1. **Add Real Project Images**: Replace emoji icons with actual project screenshots
2. **Update All Links**: Ensure all social and project links are correct
3. **Test on Mobile**: Use browser DevTools to test responsive design
4. **Optimize Images**: Compress images before deployment
5. **Add Analytics**: Integrate Google Analytics or similar
6. **Custom Domain**: Use a custom domain for professional appearance

## 🚀 Next Steps

1. Customize all personal information
2. Add your actual projects with images
3. Update skills based on your expertise
4. Test all links and forms
5. Deploy to your preferred platform
6. Share your portfolio!

---

**Built with ❤️ using Next.js, Tailwind CSS, and Framer Motion**


