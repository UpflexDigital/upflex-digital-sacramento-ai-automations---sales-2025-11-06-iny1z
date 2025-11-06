# Upflex Digital Sacramento - Landing Page Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize the Upflex Digital Sacramento landing page. Whether you're updating text, fixing links, or adding new sections, you'll find detailed instructions below.

---

## Table of Contents

1. [Quick Overview](#quick-overview)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Fixing and Managing Links](#fixing-and-managing-links)
5. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
6. [Common Tasks](#common-tasks)
7. [Troubleshooting](#troubleshooting)

---

## Quick Overview

This landing page is built with:
- **HTML5** - The structure and content
- **Tailwind CSS** - A utility-first CSS framework for styling
- **Vanilla JavaScript** - For interactive elements (minimal)

**Key Files You'll Work With:**
- `index.html` - The main landing page (the file you're customizing)
- `privacy.html` - Privacy policy page (you'll create this)
- `terms.html` - Terms of service page (you'll create this)

**Color Scheme:**
- Primary (Cyan): `#00D4FF`
- Secondary (Pink): `#FF006E`
- Accent (Purple): `#8338EC`

---

## Updating Text Content

### Understanding the Page Structure

The landing page is divided into sections. Here's what each section does:

```
1. Navigation Header (top of page, stays visible)
2. Hero Section (big welcome message with buttons)
3. Features Section (3 service cards)
4. Benefits Section (3 benefit cards)
5. How It Works Section (4-step process)
6. Call-to-Action Section (main conversion section)
7. FAQ Section (frequently asked questions)
```

### How to Update Text - Step by Step

**Step 1: Open the HTML file**
- Use a text editor like Visual Studio Code, Notepad++, or even simple Notepad
- Open `index.html`

**Step 2: Find the text you want to change**
- Use `Ctrl+F` (Windows) or `Cmd+F` (Mac) to search for the text
- For example, search for "Upflex Your Digital Presence" to find the hero tagline

**Step 3: Edit the text**
- Replace the old text with your new text
- Keep HTML tags intact (don't delete `<h1>`, `<p>`, `</span>`, etc.)

**Step 4: Save the file**
- Press `Ctrl+S` (Windows) or `Cmd+S` (Mac)

---

### Specific Text Locations and How to Update Them

#### **Navigation Menu Text**
**Location:** Lines 64-70 (approximately)

**Current Code:**
```html
<a href="#features" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Features</a>
<a href="#benefits" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Benefits</a>
<a href="#cta" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Get Started</a>
<a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
```

**How to Update:**
- Find the text between `>` and `</a>`
- Change "Features" to something else if desired
- **Important:** Keep the `href="#features"` part the same unless you're also renaming the section below

**Example Change:**
```html
<!-- Old -->
<a href="#features" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Features</a>

<!-- New -->
<a href="#features" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Our Services</a>
```

---

#### **Hero Section - Main Headline**
**Location:** Lines 91-96 (approximately)

**Current Code:**
```html
<h1 class="text-5xl sm:text-6xl lg:text-7xl font-black tracking-tight leading-tight">
    <span class="block text-white">Upflex Digital</span>
    <span class="block gradient-text mt-2">Sacramento</span>
</h1>
```

**How to Update:**
- The first `<span>` is the first line of your headline
- The second `<span>` is the second line with the gradient colors
- Change the text inside the `<span>` tags

**Example Change:**
```html
<h1 class="text-5xl sm:text-6xl lg:text-7xl font-black tracking-tight leading-tight">
    <span class="block text-white">Your Company Name</span>
    <span class="block gradient-text mt-2">Your City</span>
</h1>
```

---

#### **Hero Section - Tagline**
**Location:** Lines 98-100 (approximately)

**Current Code:**
```html
<p class="text-2xl sm:text-3xl lg:text-4xl font-bold text-cyan-400 animate-slide-up">
    AI Automations & Sales
</p>
```

**How to Update:**
- Change the text between `<p>` and `</p>`
- Keep the class names the same

**Example Change:**
```html
<p class="text-2xl sm:text-3xl lg:text-4xl font-bold text-cyan-400 animate-slide-up">
    Digital Solutions for Growth
</p>
```

---

#### **Hero Section - Description**
**Location:** Lines 105-107 (approximately)

**Current Code:**
```html
<p class="text-lg text-gray-400 max-w-2xl mx-auto leading-relaxed">
    Transform your business with cutting-edge AI solutions, stunning web design, and powerful social media marketing automation.
</p>
```

**How to Update:**
- Change the text between `<p>` and `</p>`
- This is where you explain what you do

---

#### **Feature Cards**
**Location:** Lines 154-226 (approximately)

Each feature card has three parts: Icon, Title, and Description

**Current Code Example (AI Agents Card):**
```html
<h3 class="text-2xl font-bold mb-3 text-white">AI Agents</h3>
<p class="text-gray-300 leading-relaxed">
    Intelligent automation that works 24/7 to handle customer interactions, lead qualification, and business operations with precision.
</p>
```

**How to Update:**
- Change the `<h3>` text for the title
- Change the `<p>` text for the description
- There are 3 cards: AI Agents, Web Design, and SMMA

**Example Change:**
```html
<h3 class="text-2xl font-bold mb-3 text-white">Custom Feature Name</h3>
<p class="text-gray-300 leading-relaxed">
    Your new description goes here. Keep it concise and benefit-focused.
</p>
```

---

#### **Benefits Section**
**Location:** Lines 268-330 (approximately)

Three benefit cards with titles and descriptions:

**Current Code Example:**
```html
<h3 class="text-2xl font-bold mb-3 text-white group-hover:text-cyan-400 transition-colors">Time</h3>
<p class="text-gray-400 leading-relaxed group-hover:text-gray-300 transition-colors">
    Save countless hours with intelligent automation that handles repetitive tasks...
</p>
```

**How to Update:**
- Change the `<h3>` text for the benefit title
- Change the `<p>` text for the benefit description
- Keep the class names unchanged

---

#### **FAQ Section**
**Location:** Lines 449-515 (approximately)

**Current Code Example:**
```html
<summary class="flex items-center justify-between cursor-pointer p-6 font-bold text-lg text-white hover:text-cyan-400 transition-colors duration-300">
    What is AI automation and how can it help my business?
    <span class="transform group-open:rotate-180 transition-transform duration-300">
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
        </svg>
    </span>
</summary>
<div class="px-6 pb-6 text-gray-300 leading-relaxed border-t border-gray-600">
    AI automation uses intelligent systems to handle repetitive tasks...
</div>
```

**How to Update:**
- Change the text in the `<summary>` tag for the question
- Change the text in the `<div>` tag for the answer

**Example Change:**
```html
<summary class="flex items-center justify-between cursor-pointer p-6 font-bold text-lg text-white hover:text-cyan-400 transition-colors duration-300">
    What is your service pricing?
    <span class="transform group-open:rotate-180 transition-transform duration-300">
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
        </svg>
    </span>
</summary>
<div class="px-6 pb-6 text-gray-300 leading-relaxed border-t border-gray-600">
    Our pricing varies based on your specific needs. Contact us for a custom quote.
</div>
```

---

### Important Rules When Updating Text

✅ **DO:**
- Keep all HTML tags (`<h1>`, `<p>`, `<span>`, `</div>`, etc.) exactly as they are
- Keep all `class=""` attributes exactly as they are
- Only change the text between opening and closing tags
- Save the file after making changes

❌ **DON'T:**
- Delete or move HTML tags
- Change class names
- Change the structure of the code
- Add extra spaces or line breaks that might break formatting

---

## Modifying Tailwind CSS Classes

Tailwind CSS uses a utility-first approach, meaning styling is done through class names rather than separate CSS files.

### Understanding Tailwind Classes in This Landing Page

**Common Classes You'll See:**

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-white` | Makes text white | `<h1 class="text-white">` |
| `bg-gray-900` | Dark gray background | `<div class="bg-gray-900">` |
| `text-2xl` | Large text size | `<p class="text-2xl">` |
| `font-bold` | Bold text | `<h2 class="font-bold">` |
| `rounded-lg` | Slightly rounded corners | `<button class="rounded-lg">` |
| `px-4` | Padding (left & right) | `<div class="px-4">` |
| `py-4` | Padding (top & bottom) | `<div class="py-4">` |
| `mb-4` | Margin bottom | `<div class="mb-4">` |
| `hover:text-cyan-400` | Changes color on hover | `<a class="hover:text-cyan-400">` |
| `transition-colors` | Smooth color change animation | `<a class="transition-colors">` |
| `grid grid-cols-3` | 3-column layout | `<div class="grid grid-cols-3">` |

---

### How to Change Colors

**The Color Scheme:**

This landing page uses a custom color palette defined at the top of the HTML (lines 19-24):

```html
<script>
    tailwind.config = {
        theme: {
            extend: {
                colors: {
                    primary: '#00D4FF',      /* Cyan Blue */
                    secondary: '#FF006E',    /* Pink */
                    accent: '#8338EC',       /* Purple */
                },
```

**Common Color Classes:**
- `text-cyan-400` - Cyan text
- `text-gray-300` - Light gray text
- `text-gray-900` - Dark gray (almost black)
- `bg-gray-800` - Dark gray background
- `bg-cyan-400` - Cyan background
- `border-gray-600` - Gray border

**How to Change a Color - Example:**

**Original (cyan button):**
```html
<button class="bg-cyan-400 text-gray-900 rounded-lg font-bold">
    Learn More
</button>
```

**Changed (purple button):**
```html
<button class="bg-purple-600 text-white rounded-lg font-bold">
    Learn More
</button>
```

---

### How to Change Text Size

**Text Size Classes:**
- `text-lg` - Large (18px)
- `text-xl` - Extra large (20px)
- `text-2xl` - 2x extra large (24px)
- `text-3xl` - 3x extra large (30px)
- `text-4xl` - 4x extra large (36px)
- `text-5xl` - 5x extra large (48px)
- `text-6xl` - 6x extra large (60px)
- `text-7xl` - 7x extra large (80px)

**Example - Making a heading smaller:**

**Original (very large):**
```html
<h1 class="text-5xl sm:text-6xl lg:text-7xl font-black">
    Upflex Digital
</h1>
```

**Changed (smaller):**
```html
<h1 class="text-4xl sm:text-5xl lg:text-6xl font-black">
    Upflex Digital
</h1>
```

---

### How to Change Spacing (Padding & Margins)

**Padding Classes (space inside an element):**
- `p-4` - Padding all around (16px)
- `px-4` - Padding left & right (16px)
- `py-4` - Padding top & bottom (16px)
- `pt-4` - Padding top only
- `pb-4` - Padding bottom only

**Margin Classes (space outside an element):**
- `m-4` - Margin all around (16px)
- `mx-4` - Margin left & right (16px)
- `my-4` - Margin top & bottom (16px)
- `mb-4` - Margin bottom (16px)
- `mt-4` - Margin top (16px)

**Example - Adding more space around a button:**

**Original:**
```html
<button class="px-8 py-4 rounded-lg font-bold">
    Start Now
</button>
```

**With more padding:**
```html
<button class="px-12 py-6 rounded-lg font-bold">
    Start Now
</button>
```

---

### How to Change Border Radius (Rounded Corners)

**Border Radius Classes:**
- `rounded-none` - No rounding
- `rounded-sm` - Slight rounding
- `rounded-lg` - Medium rounding
- `rounded-xl` - Large rounding
- `rounded-2xl` - Extra large rounding
- `rounded-full` - Completely circular

**Example - Making corners more rounded:**

**Original (medium rounding):**
```html
<div class="rounded-lg bg-gray-800">
    Content here
</div>
```

**Changed (more rounded):**
```html
<div class="rounded-2xl bg-gray-800">
    Content here
</div>
```

---

### How to Change Responsive Behavior

This page uses responsive design, meaning it looks good on phones, tablets, and desktops.

**Responsive Prefixes:**
- `sm:` - Small screens (640px and up)
- `md:` - Medium screens (768px and up)
- `lg:` - Large screens (1024px and up)

**Example - Text that gets bigger on larger screens:**
```html
<h1 class="text-4xl sm:text-5xl lg:text-6xl">
    Upflex Digital
</h1>
```

This means:
- On mobile: `text-4xl` (36px)
- On tablets: `text-5xl` (48px)
- On desktops: `text-6xl` (60px)

---

### Custom CSS in This Landing Page

Some styling is done with custom CSS (lines 44-68). Here's what each does:

```css
.gradient-text {
    /* Creates the rainbow gradient text effect */
    background: linear-gradient(135deg, #00D4FF 0%, #FF006E 50%, #8338EC 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
}

.hover-glow:hover {
    /* Adds a glowing effect when you hover over buttons */
    box-shadow: 0 0 30px rgba(0, 212, 255, 0.4);
}

.btn-primary {
    /* Main button styling with gradient background */
    background: linear-gradient(135deg, #00D4FF 0%, #8338EC 100%);
    transition: all 0.3s ease;
}

.btn-primary:hover {
    /* Button effect on hover */
    transform: scale(1.05);
    box-shadow: 0 10px 40px rgba(0, 212, 255, 0.3);
}

.card-hover {
    /* Smooth transitions for cards */
    transition: all 0.3s ease;
}

.card-hover:hover {
    /* Card lifts up when you hover */
    transform: translateY(-10px);
    box-shadow: 0 20px 50px rgba(0, 212, 255, 0.2);
}
```

**When to modify these:**
- Only edit if you want to change how buttons or cards behave
- Keep the structure the same, only change colors and values

---

## Fixing and Managing Links

Links are crucial for navigation. This section shows you how to find and fix them.

### Understanding Link Types

**Internal Links** (link to sections on the same page):
```html
<a href="#features">Features</a>  <!-- Takes you to id="features" -->
```

**External Links** (link to other websites):
```html
<a href="https://upflexdigital.com">Visit Website</a>
```

**Email Links:**
```html
<a href="mailto:info@upflexdigital.com">Email Us</a>
```

---

### All Links in This Landing Page

Here's every link in the current landing page:

| Location | Current Link | Type | Purpose |
|----------|-------------|------|---------|
| Navigation - Features | `#features` | Internal | Jumps to Features section |
| Navigation - Benefits | `#benefits` | Internal | Jumps to Benefits section |
| Navigation - Get Started | `#cta` | Internal | Jumps to CTA section |
| Navigation - Contact | `mailto:info@upflexdigital.com` | Email | Opens email client |
| Hero - Main Button | `https://upflexdigital.com` | External | Main website |
| Hero - Learn More Button | None (button only) | None | Currently doesn't go anywhere |
| CTA - Consultation Button | `https://upflexdigital.com` | External | Main website |
| CTA - Contact Button | `mailto:info@upflexdigital.com` | Email | Opens email client |

---

### How to Update External Links

**Step 1: Find the link you want to change**

Example - Hero section main button (line 113):
```html
<a href="https://upflexdigital.com" class="btn-primary px-8 py-4 rounded-lg font-bold text-lg text-white inline-block hover-glow focus:outline-none focus:ring-2 focus:ring-cyan-400 focus:ring-offset-2 focus:ring-offset-gray-900">
    Start Your Transformation
</a>
```

**Step 2: Change the `href` value**

Replace the URL between the quotes:
```html
<!-- Old -->
<a href="https://upflexdigital.com" class="...">

<!-- New -->
<a href="https://yourdomain.com" class="...">
```

**Step 3: Save and test**

- Save the file
- Click the link to make sure it works

---

### How to Update Email Links

**Current email link:**
```html
<a href="mailto:info@upflexdigital.com">Contact</a>
```

**To change the email:**
```html
<a href="mailto:your-email@yourdomain.com">Contact</a>
```

---

### How to Update Internal Links (Anchor Links)

**What are anchor links?**
Anchor links jump to a specific section on the same page. They use the `#` symbol.

**Current internal links:**
```html
<a href="#features">Features</a>     <!-- Links to id="features" -->
<a href="#benefits">Benefits</a>     <!-- Links to id="benefits" -->
<a href="#cta">Get Started</a>       <!-- Links to id="cta" -->
```

**The matching section IDs:**
```html
<section id="features" class="py-24 bg-gray-800 border-t border-gray-700">
    <!-- Features section content -->
</section>

<section id="benefits" class="py-24 bg-gray-900 border-t border-gray-700">
    <!-- Benefits section content -->
</section>

<section id="cta" class="relative py-24 overflow-hidden">
    <!-- CTA section content -->
</section>
```

**How they work together:**
- Navigation link `href="#features"` takes you to the section with `id="features"`
- The names must match exactly (case-sensitive)

**If you rename a section:**

1. Change the `id` in the section:
```html
<!-- Old -->
<section id="features" class="...">

<!-- New -->
<section id="our-services" class="...">
```

2. Update the navigation link:
```html
<!-- Old -->
<a href="#features">Features</a>

<!-- New -->
<a href="#our-services">Our Services</a>
```

---

### How to Fix the "Learn More" Button

Currently, the "Learn More" button in the Hero section doesn't have a link. Here's how to fix it:

**Current code (line 117):**
```html
<button class="px-8 py-4 rounded-lg font-bold text-lg text-cyan-400 border-2 border-cyan-400 hover:bg-cyan-400 hover:text-gray-900 transition-all duration-300 focus:outline-none focus:ring-2 focus:ring-cyan-400 focus:ring-offset-2 focus:ring-offset-gray-900">
    Learn More
</button>
```

**Change it to a link:**
```html
<a href="#features" class="px-8 py-4 rounded-lg font-bold text-lg text-cyan-400 border-2 border-cyan-400 hover:bg-cyan-400 hover:text-gray-900 transition-all duration-300 focus:outline-none focus:ring-2 focus:ring-cyan-400 focus:ring-offset-2 focus:ring-offset-gray-900 inline-block">
    Learn More
</a>
```

**What changed:**
- Changed `<button>` to `<a>`
- Added `href="#features"` to link to the Features section
- Changed `</button>` to `</a>`
- Added `inline-block` class to make it display like a button

---

### Testing Links - Checklist

After updating links, test them:

- [ ] Click each navigation link - does it jump to the right section?
- [ ] Click each button - does it go to the right place?
- [ ] Click the email link - does it open your email client?
- [ ] Click external links - do they open the right website?
- [ ] Try on mobile - do links work on phones?

---

## Adding Privacy and Terms Pages

Most websites need Privacy Policy and Terms of Service pages. Here's how to add them and link them properly.

### Step 1: Create the Privacy Policy Page

**Step 1a: Create a new file**
- Right-click in your project folder
- Select "New File" or "Create File"
- Name it `privacy.html`

**Step 1b: Copy this template into privacy.html:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Upflex Digital Sacramento">
    <meta name="author" content="Upflex Digital">
    <title>Privacy Policy - Upflex Digital Sacramento</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 bg-gradient-to-r from-blue-500 to-purple-600 rounded-lg flex items-center justify-center">
                    <span class="text-white font-bold text-lg">U</span>
                </div>
                <span class="text-xl font-bold text-white">Upflex</span>
            </div>
            
            <div class="hidden md:flex items-center space-x-8">
                <a href="index.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Home</a>
                <a href="privacy.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Privacy</a>
                <a href="terms.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Terms</a>
                <a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
            </div>
            
            <button class="md:hidden text-gray-300 hover:text-cyan-400 focus:outline-none" aria-label="Toggle menu">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                </svg>
            </button>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-black text-white mb-8">Privacy Policy</h1>
            
            <div class="prose prose-invert max-w-none space-y-6 text-gray-300">
                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Introduction</h2>
                    <p>
                        At Upflex Digital Sacramento, we are committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Information We Collect</h2>
                    <p>
                        We may collect information about you in a variety of ways. The information we may collect on the site includes:
                    </p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Name</li>
                        <li>Email address</li>
                        <li>Phone number</li>
                        <li>Company name</li>
                        <li>Information about your business needs</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">How We Use Your Information</h2>
                    <p>
                        Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the site to:
                    </p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Generate leads and respond to inquiries</li>
                        <li>Send periodic emails regarding your order or other products and services</li>
                        <li>Follow up with you after correspondence</li>
                        <li>Improve our website and services</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Security of Your Information</h2>
                    <p>
                        We use administrative, technical, and physical security measures to help protect your personal information. While we have taken reasonable steps to secure the personal information you provide to us, please be aware that no security measures are perfect or impenetrable.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Contact Us</h2>
                    <p>
                        If you have questions or comments about this Privacy Policy, please contact us at:
                    </p>
                    <p class="text-cyan-400">
                        Email: <a href="mailto:info@upflexdigital.com" class="hover:text-cyan-300">info@upflexdigital.com</a>
                    </p>
                </section>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 border-t border-gray-700 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-gray-400">
            <p>&copy; 2024 Upflex Digital Sacramento. All rights reserved.</p>
            <div class="mt-4 space-x-4">
                <a href="privacy.html" class="text-gray-300 hover:text-cyan-400 transition-colors">Privacy Policy</a>
                <span>|</span>
                <a href="terms.html" class="text-gray-300 hover:text-cyan-400 transition-colors">Terms of Service</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

---

### Step 2: Create the Terms of Service Page

**Step 2a: Create a new file**
- Right-click in your project folder
- Select "New File"
- Name it `terms.html`

**Step 2b: Copy this template into terms.html:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Upflex Digital Sacramento">
    <meta name="author" content="Upflex Digital">
    <title>Terms of Service - Upflex Digital Sacramento</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        * {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 bg-gradient-to-r from-blue-500 to-purple-600 rounded-lg flex items-center justify-center">
                    <span class="text-white font-bold text-lg">U</span>
                </div>
                <span class="text-xl font-bold text-white">Upflex</span>
            </div>
            
            <div class="hidden md:flex items-center space-x-8">
                <a href="index.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Home</a>
                <a href="privacy.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Privacy</a>
                <a href="terms.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Terms</a>
                <a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
            </div>
            
            <button class="md:hidden text-gray-300 hover:text-cyan-400 focus:outline-none" aria-label="Toggle menu">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                </svg>
            </button>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-black text-white mb-8">Terms of Service</h1>
            
            <div class="prose prose-invert max-w-none space-y-6 text-gray-300">
                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Agreement to Terms</h2>
                    <p>
                        By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Use License</h2>
                    <p>
                        Permission is granted to temporarily download one copy of the materials (information or software) on Upflex Digital's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                    </p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Modify or copy the materials</li>
                        <li>Use the materials for any commercial purpose or for any public display</li>
                        <li>Attempt to decompile or reverse engineer any software contained on the website</li>
                        <li>Remove any copyright or other proprietary notations from the materials</li>
                        <li>Transfer the materials to another person or "mirror" the materials on any other server</li>
                    </ul>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Disclaimer</h2>
                    <p>
                        The materials on Upflex Digital's website are provided on an 'as is' basis. Upflex Digital makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Limitations</h2>
                    <p>
                        In no event shall Upflex Digital or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Upflex Digital's website.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Accuracy of Materials</h2>
                    <p>
                        The materials appearing on Upflex Digital's website could include technical, typographical, or photographic errors. Upflex Digital does not warrant that any of the materials on its website are accurate, complete, or current.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Modifications</h2>
                    <p>
                        Upflex Digital may revise these terms of service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                    </p>
                </section>

                <section>
                    <h2 class="text-3xl font-bold text-white mb-4">Contact Us</h2>
                    <p>
                        If you have questions about these Terms of Service, please contact us at:
                    </p>
                    <p class="text-cyan-400">
                        Email: <a href="mailto:info@upflexdigital.com" class="hover:text-cyan-300">info@upflexdigital.com</a>
                    </p>
                </section>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 border-t border-gray-700 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-gray-400">
            <p>&copy; 2024 Upflex Digital Sacramento. All rights reserved.</p>
            <div class="mt-4 space-x-4">
                <a href="privacy.html" class="text-gray-300 hover:text-cyan-400 transition-colors">Privacy Policy</a>
                <span>|</span>
                <a href="terms.html" class="text-gray-300 hover:text-cyan-400 transition-colors">Terms of Service</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

---

### Step 3: Add Links to Privacy and Terms in index.html

Now you need to add links to these pages in your main landing page. There are several places you can add them:

#### **Option 1: Add to Navigation Menu (Recommended)**

**Find this code (around line 64-70):**
```html
<div class="hidden md:flex items-center space-x-8">
    <a href="#features" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Benefits</a>
    <a href="#cta" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Get Started</a>
    <a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
</div>
```

**Change it to:**
```html
<div class="hidden md:flex items-center space-x-8">
    <a href="#features" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Benefits</a>
    <a href="#cta" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Get Started</a>
    <a href="privacy.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Privacy</a>
    <a href="terms.html" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Terms</a>
    <a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
</div>
```

---

#### **Option 2: Add to Footer (Most Common)**

Add a footer to your `index.html` just before the closing `</body>` tag:

**Find this line near the end (should be the last line before `</body>`):**
```html
</section>
```

**Add this footer code right before `</body>`:**
```html
    <!-- Footer -->
    <footer class="bg-gray-800 border-t border-gray-700 py-8">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center text-gray-400">
            <p>&copy; 2024 Upflex Digital Sacramento. All rights reserved.</p>
            <div class="mt-4 space-x-4">
                <a href="privacy.html" class="text-gray-300 hover:text-cyan-400 transition-colors">Privacy Policy</a>
                <span>|</span>
                <a href="terms.html" class="text-gray-300 hover:text-cyan-400 transition-colors">Terms of Service</a>
            </div>
        </div>
    </footer>

</body>
</html>
```

---

### Step 4: Customize Your Privacy and Terms Pages

The templates above are generic. You should customize them with your specific information:

**In privacy.html, update:**
- Your actual privacy practices
- What data you collect
- How you use it
- Your email address
- Your company name and location

**In terms.html, update:**
- Your specific terms and conditions
- Liability disclaimers
- Usage restrictions
- Your email address
- Your company name and location

---

### Step 5: Test the Links

1. Open `index.html` in your browser
2. Click the Privacy Policy link - it should take you to `privacy.html`
3. Click the Terms of Service link - it should take you to `terms.html`
4. From those pages, click the "Home" link - it should return to `index.html`
5. Try on mobile to ensure links work on smaller screens

---

## Common Tasks

### Task 1: Change Your Company Name Throughout the Page

**Places where "Upflex Digital" appears:**

1. **Page title (line 6):**
```html
<title>Upflex Digital Sacramento - AI Automations & Sales</title>
```

2. **Meta description (line 5):**
```html
<meta name="description" content="Upflex Digital Sacramento - AI Automations & Sales...">
```

3. **Logo/Brand in navigation (line 67):**
```html
<span class="text-xl font-bold text-white">Upflex</span>
```

4. **Hero section heading (line 93-94):**
```html
<span class="block text-white">Upflex Digital</span>
```

5. **Footer copyright (in footer you add):**
```html
<p>&copy; 2024 Upflex Digital Sacramento. All rights reserved.</p>
```

**To change all of these:**
- Use `Ctrl+H` (Windows) or `Cmd+H` (Mac) to "Find and Replace"
- Find: `Upflex Digital`
- Replace with: `Your Company Name`
- Click "Replace All"

---

### Task 2: Change Your Email Address

**Current email:** `info@upflexdigital.com`

**Places it appears:**
- Navigation contact link (line 70)
- Hero section (line 118)
- CTA section (line 435)
- FAQ section (line 512)

**To change:**
- Use `Ctrl+H` or `Cmd+H`
- Find: `info@upflexdigital.com`
- Replace with: `your-email@yourdomain.com`
- Click "Replace All"

---

### Task 3: Change Your City/Location

**Current location:** `Sacramento`

**Places it appears:**
- Page title
- Meta description
- Hero heading
- CTA section text

**To change:**
- Use Find and Replace
- Find: `Sacramento`
- Replace with: `Your City`
- Review each replacement to make sure it's appropriate

---

### Task 4: Add a New FAQ Item

**Find the FAQ section (around line 449)**

**Current structure:**
```html
<details class="group bg-gray-700 rounded-lg overflow-hidden border border-gray-600 hover:border-cyan-400 transition-colors duration-300">
    <summary class="flex items-center justify-between cursor-pointer p-6 font-bold text-lg text-white hover:text-cyan-400 transition-colors duration-300">
        Question here?
        <span class="transform group-open:rotate-180 transition-transform duration-300">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
            </svg>
        </span>
    </summary>
    <div class="px-6 pb-6 text-gray-300 leading-relaxed border-t border-gray-600">
        Answer here.
    </div>
</details>
```

**To add a new FAQ:**
1. Copy the entire `<details>` block above
2. Paste it after the last FAQ item
3. Change the question in the `<summary>` tag
4. Change the answer in the `<div>` tag
5. Optionally change the hover color (cyan-400 to purple-400 or pink-400)

---

### Task 5: Change Button Colors

**Primary button (cyan):**
```html
<a href="..." class="btn-primary px-8 py-4 rounded-lg ...">
    Button Text
</a>
```

The `.btn-primary` class controls the color. To change it, find the CSS (around line 52):

```css
.btn-primary {
    background: linear-gradient(135deg, #00D4FF 0%, #8338EC 100%);
    transition: all 0.3s ease;
}
```

**To change to purple:**
```css
.btn-primary {
    background: linear-gradient(135deg, #8338EC 0%, #FF006E 100%);
    transition: all 0.3s ease;
}
```

---

### Task 6: Add Your Phone Number

**Add a phone link to the navigation:**

Find the contact link in navigation (around line 70):
```html
<a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
```

Add a phone link before or after it:
```html
<a href="tel:+1-916-555-1234" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Call Us</a>
<a href="mailto:info@upflexdigital.com" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300 font-medium">Contact</a>
```

Replace `+1-916-555-1234` with your actual phone number (format: `+1-area-exchange-number`).

---

### Task 7: Change Feature Card Icons

Each feature card has an icon. The icons are SVG code. To change them:

**Find a feature card (around line 161):**
```html
<svg class="w-8 h-8 text-white" fill="currentColor" viewBox="0 0 20 20">
    <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v4h8v-4zM6 8a2 2 0 11-4 0 2 2 0 014 0zM16 18v-3a5.972 5.972 0 00-.75-2.906A3.005 3.005 0 0119 15v3h-3zM4.75 12.094A5.973 5.973 0 004 15v3H1v-3a3 3 0 013.75-2.906z"></path>
</svg>
```

**To use a different icon:**
1. Visit [Heroicons](https://heroicons.com/) (free SVG icons)
2. Find an icon you like
3. Copy the SVG code
4. Replace the old `<svg>` section with the new one

---

## Troubleshooting

### Problem: Links aren't working

**Possible causes and solutions:**

1. **Typo in the URL**
   - Check that you typed the URL correctly
   - Make sure there are no extra spaces
   - Example: `https://upflexdigital.com` (not `https://upflexdigital.com ` with a space)

2. **Internal link points to non-existent section**
   - Make sure the `href="#features"` matches an `id="features"` in the HTML
   - IDs are case-sensitive: `#Features` is different from `#features`

3. **File path is wrong**
   - If linking to `privacy.html`, make sure the file is in the same folder as `index.html`
   - If files are in different folders, use the correct path: `pages/privacy.html`

**Quick checklist:**
- [ ] Is the `href` attribute present?
- [ ] Is the URL spelled correctly?
- [ ] For internal links, does the `id` match the `href`?
- [ ] For external links, does the URL start with `https://`?
- [ ] For email links, does it start with `mailto:`?

---

### Problem: Text looks cut off or weird on mobile

**Possible causes:**

1. **Text size is too large for small screens**
   - Look for classes like `text-6xl` or `text-7xl`
   - Add responsive versions: `text-4xl sm:text-5xl lg:text-6xl`

2. **Container is too narrow**
   - Check for `max-w-` classes
   - Make sure padding (`px-`) is appropriate

**Example fix:**
```html
<!-- Before (too large on mobile) -->
<h1 class="text-7xl font-bold">Big Headline</h1>

<!-- After (responsive) -->
<h1 class="text-3xl sm:text-5xl lg:text-7xl font-bold">Big Headline</h1>
```

---

### Problem: Colors look different than expected

**Possible causes:**

1. **Browser cache**
   - Hard refresh: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)

2. **Wrong color class used**
   - Check that you used the right color name
   - Available colors: `cyan-400`, `purple-400`, `pink-400`, `gray-300`, etc.

3. **Gradient text not working**
   - Make sure you're using the `gradient-text` class
   - This class has special styling in the `<style>` section

---

### Problem: Layout is broken or elements are overlapping

**Possible causes:**

1. **Accidentally deleted or modified a class**
   - Check that all `class=""` attributes are still complete
   - Don't remove responsive prefixes like `md:` or `lg:`

2. **Deleted a `<div>` tag**
   - Make sure all opening `<div>` tags have matching closing `</div>` tags

**To fix:**
1. Use `Ctrl+Z` to undo recent changes
2. Check that all HTML tags match (open and close properly)
3. Validate your HTML at [W3C Validator](https://validator.w3.org/)

---

### Problem: Buttons aren't clickable or styled correctly

**Possible causes:**

1. **Changed a link to a button accidentally**
   - Links use `<a>` tags, buttons use `<button>` tags
   - For navigation, use `<a>` tags with `href`

2. **Removed important classes**
   - Make sure you kept all the class names
   - Example: `class="px-8 py-4 rounded-lg font-bold text-lg ..."`

**Correct button structure:**
```html
<a href="https://example.com" class="btn-primary px-8 py-4 rounded-lg font-bold text-lg text-white inline-block">
    Click Me
</a>
```

---

### Problem: Animation isn't smooth or is glitchy

**Possible causes:**

1. **Removed transition classes**
   - Look for `transition-colors`, `transition-all`, etc.
   - These make animations smooth

2. **Changed animation duration**
   - Look for `duration-300`, `duration-500`, etc.
   - Longer durations = slower animations

**Example - smooth transition:**
```html
<a href="#" class="text-gray-300 hover:text-cyan-400 transition-colors duration-300">
    Link
</a>
```

---

### Problem: Page loads slowly

**Possible causes:**

1. **Large background images**
   - The CTA section uses a background image from Unsplash
   - Consider replacing with a smaller image or removing it

2. **Too many animations**
   - Reduce the number of animated elements
   - Remove `animate-fade-in`, `animate-slide-up` classes if needed

**To optimize:**
- Compress images before using them
- Limit animations to important elements
- Remove unused CSS classes

---

### Problem: Can't find where to edit something

**Solution: Use Find and Replace**

1. Press `Ctrl+F` (Windows) or `Cmd+F` (Mac)
2. Type the text you're looking for
3. The editor will highlight all matches
4. Use the arrow buttons to navigate between matches

**Example:** Want to find all instances of "AI Agents"?
- Press `Ctrl+F`
- Type: `AI Agents`
- All instances will be highlighted

---

## File Organization

**Recommended folder structure:**

```
your-website/
├── index.html           (main landing page)
├── privacy.html         (privacy policy)
├── terms.html           (terms of service)
├── css/
│   └── custom.css       (optional: additional styles)
├── images/
│   ├── logo.png
│   └── hero-image.jpg
└── README.md            (this file)
```

---

## Best Practices

✅ **DO:**
- Back up your files before making major changes
- Test all links after updating them
- Check the page on mobile devices
- Use descriptive file names
- Keep consistent styling across all pages
- Update your email and contact info in all places
- Test on different browsers (Chrome, Firefox, Safari, Edge)

❌ **DON'T:**
- Edit multiple things at once without testing
- Delete HTML tags without understanding them
- Change class names randomly
- Add too many custom styles
- Leave broken links on your site
- Forget to save your changes
- Test only on desktop

---

## Getting Help

**If you're stuck:**

1. **Check this guide** - Use Ctrl+F to search for your issue
2. **Use browser developer tools** - Right-click → Inspect → Check for errors
3. **Validate your HTML** - Visit [W3C Validator](https://validator.w3.org/)
4. **Search online** - Search for "Tailwind CSS [your question]" or "HTML [your question]"
5. **Contact support** - Reach out to `info@upflexdigital.com`

---

## Summary

You now know how to:
- ✅ Update text content throughout the page
- ✅ Modify Tailwind CSS classes for styling
- ✅ Fix and manage links
- ✅ Add privacy and terms pages
- ✅ Perform common customization tasks
- ✅ Troubleshoot common issues

**Next steps:**
1. Make a backup of your files
2. Start with small changes (like updating your company name)
3. Test each change in your browser
4. Gradually customize the page to match your brand
5. Deploy your site when you're happy with it

Good luck with your Upflex Digital landing page! 🚀