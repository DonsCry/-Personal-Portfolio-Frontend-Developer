# Complete Setup & Deployment Guide

## 🚀 Quick Start

### PROJECT 3 - Main Portfolio Website

```bash
# Navigate to root
cd c:\xampp\htdocs\projectweb\portofolio-me

# Install dependencies
npm install

# Start development server
npm run dev

# Visit http://localhost:3000
```

### PROJECT 4 - Travel Booking UI

```bash
# Navigate to project
cd c:\xampp\htdocs\projectweb\portofolio-me\projects\travel-booking

# Install dependencies
npm install

# Start development server
npm run dev

# Visit http://localhost:3000
```

### PROJECT 5 - Apple Clone

```bash
# Navigate to project
cd c:\xampp\htdocs\projectweb\portofolio-me\projects\apple-clone

# Install dependencies
npm install

# Start development server
npm run dev

# Visit http://localhost:3000
```

---

## 📋 Project Structure

```
portofolio-me/
│
├── 📄 README.md                    # Main portfolio documentation
├── 📄 PROJECTS.md                  # All projects overview
├── 📄 SETUP_GUIDE.md              # This file
├── 📄 package.json                # Dependencies
├── 📄 tsconfig.json               # TypeScript config
├── 📄 tailwind.config.js          # Tailwind config
├── 📄 postcss.config.js           # PostCSS config
├── 📄 next.config.js              # Next.js config
│
├── 📁 app/                         # PROJECT 3 - Main Portfolio
│   ├── layout.tsx
│   ├── page.tsx
│   └── globals.css
│
├── 📁 components/                  # PROJECT 3 Components
│   ├── Navbar.tsx
│   ├── Hero.tsx
│   ├── Projects.tsx
│   ├── Skills.tsx
│   ├── Contact.tsx
│   └── Footer.tsx
│
└── 📁 projects/
    │
    ├── 📁 travel-booking/          # PROJECT 4 - Travel Booking UI
    │   ├── app/
    │   ├── components/
    │   ├── package.json
    │   ├── tsconfig.json
    │   ├── tailwind.config.js
    │   ├── postcss.config.js
    │   ├── next.config.js
    │   └── README.md
    │
    └── 📁 apple-clone/             # PROJECT 5 - Apple Clone
        ├── app/
        ├── components/
        ├── package.json
        ├── tsconfig.json
        ├── tailwind.config.js
        ├── postcss.config.js
        ├── next.config.js
        └── README.md
```

---

## 🛠️ Installation Steps

### Prerequisites
- Node.js 18+ installed
- npm or yarn package manager
- Git (for version control)

### Step 1: Clone or Navigate to Project
```bash
cd c:\xampp\htdocs\projectweb\portofolio-me
```

### Step 2: Install Main Portfolio Dependencies
```bash
npm install
```

### Step 3: Install Sub-Project Dependencies
```bash
# Travel Booking
cd projects/travel-booking && npm install && cd ../..

# Apple Clone
cd projects/apple-clone && npm install && cd ../..
```

### Step 4: Verify Installation
```bash
npm run dev
# Should start on http://localhost:3000
```

---

## 🎯 Development Workflow

### Running All Projects Locally

**Terminal 1 - Main Portfolio (Port 3000)**
```bash
npm run dev
```

**Terminal 2 - Travel Booking (Port 3001)**
```bash
cd projects/travel-booking
npm run dev -- -p 3001
```

**Terminal 3 - Apple Clone (Port 3002)**
```bash
cd projects/apple-clone
npm run dev -- -p 3002
```

### Access Points
- Main Portfolio: http://localhost:3000
- Travel Booking: http://localhost:3001
- Apple Clone: http://localhost:3002

---

## 🔧 Configuration

### Environment Variables
Create `.env.local` in each project root (if needed):

```env
# .env.local
NEXT_PUBLIC_API_URL=http://localhost:3000
```

### Tailwind Configuration
Already configured in `tailwind.config.js` for each project.

### TypeScript
Already configured in `tsconfig.json` for each project.

---

## 📦 Build & Production

### Build Main Portfolio
```bash
npm run build
npm start
```

### Build Travel Booking
```bash
cd projects/travel-booking
npm run build
npm start
```

### Build Apple Clone
```bash
cd projects/apple-clone
npm run build
npm start
```

---

## 🚀 Deployment Options

### Option 1: Deploy to Vercel (Recommended)

**Install Vercel CLI:**
```bash
npm install -g vercel
```

**Deploy Main Portfolio:**
```bash
vercel
```

**Deploy Travel Booking:**
```bash
cd projects/travel-booking
vercel
```

**Deploy Apple Clone:**
```bash
cd projects/apple-clone
vercel
```

### Option 2: Deploy to Netlify

**Main Portfolio:**
1. Push to GitHub
2. Go to netlify.com
3. Click "New site from Git"
4. Select repository
5. Build command: `npm run build`
6. Publish directory: `.next`

**Sub-Projects:**
Same process, but select the subdirectory as the base directory.

### Option 3: Deploy to GitHub Pages

```bash
# Build
npm run build
npm run export

# Push to gh-pages branch
git add .
git commit -m "Deploy"
git push origin main
```

---

## 🔍 Troubleshooting

### Issue: Dependencies not installing
```bash
# Clear npm cache
npm cache clean --force

# Delete node_modules
rm -r node_modules

# Reinstall
npm install
```

### Issue: Port already in use
```bash
# Use different port
npm run dev -- -p 3001
```

### Issue: TypeScript errors
```bash
# Rebuild TypeScript
npm run build

# Check for type errors
npx tsc --noEmit
```

### Issue: Tailwind styles not loading
```bash
# Rebuild Tailwind
npm run dev

# Clear Next.js cache
rm -r .next
npm run dev
```

---

## 📝 Customization Guide

### PROJECT 3 - Main Portfolio

**Update Hero Section:**
```typescript
// components/Hero.tsx
- Change headline text
- Update social links
- Modify CTA buttons
```

**Add Your Projects:**
```typescript
// components/Projects.tsx
const projects = [
  {
    id: 1,
    title: 'Your Project',
    description: 'Your description',
    role: 'Your role',
    tech: ['React', 'Tailwind'],
    image: '🎨',
    demo: 'https://your-demo.com',
    github: 'https://github.com/your-repo',
  },
  // Add more...
]
```

**Update Skills:**
```typescript
// components/Skills.tsx
const skills = [
  { category: 'Frontend', items: ['React', 'Next.js', 'Your Skills'] },
  // Add more categories...
]
```

**Update Contact Info:**
```typescript
// components/Contact.tsx
- Email: your@email.com
- WhatsApp: +1 (234) 567-890
- GitHub: github.com/yourprofile
- LinkedIn: linkedin.com/in/yourprofile
```

### PROJECT 4 - Travel Booking

**Update Destinations:**
```typescript
// components/FeaturedDestinations.tsx
const destinations = [
  {
    id: 1,
    name: 'Your Destination',
    image: '🏖️',
    rating: 4.8,
    reviews: 2543,
    price: '$899',
    description: 'Your description',
  },
  // Add more...
]
```

**Update Deals:**
```typescript
// components/PopularDeals.tsx
const deals = [
  {
    id: 1,
    title: 'Your Deal',
    discount: '-40%',
    originalPrice: '$1,299',
    finalPrice: '$779',
    duration: '7 days',
    image: '🏖️',
  },
  // Add more...
]
```

### PROJECT 5 - Apple Clone

**Update Products:**
```typescript
// components/ProductShowcase.tsx
const products = [
  {
    id: 1,
    name: 'Your Product',
    emoji: '💻',
    description: 'Your description',
  },
  // Add more...
]
```

**Update Features:**
```typescript
// components/Features.tsx
const features = [
  {
    icon: YourIcon,
    title: 'Your Feature',
    description: 'Your description',
  },
  // Add more...
]
```

---

## 🎨 Styling Guide

### Tailwind CSS Classes

**Common Patterns:**
```html
<!-- Responsive Grid -->
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">

<!-- Flexbox -->
<div class="flex items-center justify-between gap-4">

<!-- Spacing -->
<div class="p-6 mb-8 mt-4">

<!-- Colors -->
<div class="bg-white text-black border border-gray-200">

<!-- Hover Effects -->
<button class="hover:bg-blue-700 transition-colors">
```

### Custom Colors

**PROJECT 3 (Dark Theme):**
- Dark: `#0a0a0a`
- Secondary: `#1a1a1a`
- Accent: `#00d9ff`

**PROJECT 4 (Light Theme):**
- Primary: `#1a73e8`
- Secondary: `#f3f3f3`
- Accent: `#ea4335`

**PROJECT 5 (Premium):**
- Black: `#000000`
- White: `#ffffff`
- Gray: `#1f2937`

---

## 📊 Performance Tips

### Optimization Checklist
- ✅ Use `next/image` for images
- ✅ Lazy load components with `dynamic`
- ✅ Optimize fonts with `next/font`
- ✅ Use CSS modules for scoped styles
- ✅ Minimize bundle size
- ✅ Enable compression

### Build Optimization
```bash
# Analyze bundle
npm run build
npm run analyze  # if configured
```

---

## 🔐 Security Best Practices

- ✅ Never commit `.env.local`
- ✅ Use environment variables for secrets
- ✅ Validate all form inputs
- ✅ Sanitize user data
- ✅ Use HTTPS in production
- ✅ Keep dependencies updated

---

## 📚 Resources

### Documentation
- [Next.js Docs](https://nextjs.org/docs)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)
- [Framer Motion Docs](https://www.framer.com/motion/)
- [TypeScript Docs](https://www.typescriptlang.org/docs/)

### Tools
- [Vercel Dashboard](https://vercel.com/dashboard)
- [Netlify Dashboard](https://app.netlify.com)
- [GitHub](https://github.com)

---

## 🎓 Learning Resources

### Frontend Development
- React fundamentals
- Next.js App Router
- Tailwind CSS utilities
- Framer Motion animations

### Design
- UI/UX principles
- Responsive design
- Accessibility (WCAG)
- Performance optimization

---

## 📞 Support & Help

### Common Commands
```bash
# Development
npm run dev

# Build
npm run build

# Production
npm start

# Lint
npm run lint

# Format
npm run format  # if configured
```

### Getting Help
1. Check project README.md
2. Review PROJECTS.md
3. Check Next.js documentation
4. Search GitHub issues
5. Ask in community forums

---

## ✅ Deployment Checklist

Before deploying:
- ✅ All dependencies installed
- ✅ Environment variables configured
- ✅ Build completes without errors
- ✅ No console errors or warnings
- ✅ Responsive design tested
- ✅ All links working
- ✅ Forms validated
- ✅ Performance optimized
- ✅ SEO meta tags added
- ✅ Analytics configured (if needed)

---

## 🎉 You're Ready!

Your complete portfolio is set up and ready to deploy. Choose your deployment platform and share your work with the world!

**Happy coding! 🚀**
