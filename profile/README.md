# 💰 Informer Money — Smart Financial Guidance

> Your trusted source for personal finance, investing, and business finance insights. Expert analysis and actionable advice to help you build wealth.

[![Website](https://img.shields.io/badge/Website-informermoney.com-blue?style=flat-square&logo=google-chrome)](https://www.informermoney.com/)
[![Newsletter](https://img.shields.io/badge/Newsletter-50K%2B%20Readers-green?style=flat-square&logo=mailchimp)](https://www.informermoney.com/about#newsletter)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

---

## 📌 Table of Contents

- [Description](#-description)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Content Categories](#-content-categories)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 📖 Description

**Informer Money** is a modern, content-driven personal finance platform designed to deliver smart financial guidance to everyday readers. The platform covers a wide spectrum of financial topics — from budgeting and investing to tax strategy and entrepreneurship — presented through high-quality editorial articles authored by a team of experienced financial writers and analysts.

The platform serves over **50,000 newsletter subscribers** and is built around three core pillars:

- **Accessibility** — Financial knowledge presented in plain, actionable language.
- **Accuracy** — All content is editorially reviewed against verified financial data and current market conditions.
- **Actionability** — Every article delivers concrete, implementable guidance, not just theory.

Whether you are a first-time investor, a small business owner navigating tax season, or someone planning for retirement, Informer Money delivers the insights needed to make confident financial decisions.

> ⚠️ **Disclaimer:** Content published on Informer Money is for informational and educational purposes only. It does not constitute professional financial, investment, tax, or legal advice. Always consult a qualified professional before making financial decisions.

---

## ✨ Features

- 📰 **Editorial Blog** — Curated long-form articles across 8 financial categories, regularly updated with timely topics.
- 🔍 **Search Functionality** — Full-text search across all published articles.
- 📬 **Weekly Newsletter** — Curated financial insights delivered to 50,000+ subscribers every week, ad-free.
- 📂 **Category Browsing** — Topic-based navigation for focused reading experiences.
- 📱 **Responsive Design** — Fully optimized for desktop and mobile reading.
- 🏷️ **Trending & Editor's Picks** — Surfaced content recommendations based on editorial judgment and reader engagement.
- 🔒 **Privacy-First** — No data sales; newsletter subscribers can unsubscribe at any time.

---

## 🛠️ Tech Stack

> *The following reflects the inferred technical architecture based on observable platform behavior. Update this section to match your actual implementation.*

| Layer         | Technology                                            |
|---------------|-------------------------------------------------------|
| Frontend      | Next.js (React)                                       |
| CMS / Content | Sanity.io (headless CMS)                              |
| Styling       | Tailwind CSS                                          |
| Analytics     | Google Tag Manager, Google Analytics, Umami Analytics |
| SEO           | Next.js metadata API                                  |
| Deployment    | Vercel (inferred)                                     |
| Newsletter    | Third-party ESP (e.g., Mailchimp)                     |
| Image CDN     | Sanity CDN                                            |

---

## ⚙️ Installation

Follow these steps to run the project locally:

### Prerequisites

Ensure you have the following installed on your system:

- [Node.js](https://nodejs.org/) `v18.x` or higher
- [npm](https://www.npmjs.com/) `v9.x` or higher (or `yarn` / `pnpm`)
- A [Sanity.io](https://www.sanity.io/) account and project (if using the CMS)

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Informer-Money.git
   cd informer-money
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Copy the example environment file and populate it with your credentials:

   ```bash
   cp .env.example .env.local
   ```

   Required variables:

   ```env
   NEXT_PUBLIC_SANITY_PROJECT_ID=your_sanity_project_id
   NEXT_PUBLIC_SANITY_DATASET=production
   SANITY_API_TOKEN=your_sanity_api_token
   NEXT_PUBLIC_SITE_URL=http://localhost:3000
   NEXT_PUBLIC_GTM_ID=your_gtm_id
   ```

4. **Run the development server:**

   ```bash
   pnpm run dev
   ```

5. **Open in your browser:**

   ```
   http://localhost:3000
   ```

### Build for Production

```bash
pnpm run build
pnpm start
```

### Run Linting & Tests

```bash
# Lint
pnpm run lint

# Tests (if configured)
pnpm run test
```

---

## 🚀 Usage

### Browsing Articles

Navigate to the **Blog** section to browse all published content, or use the **Category** navigation to filter by topic:

```
https://www.informermoney.com/blog
https://www.informermoney.com/category/investing
```

### Searching Content

Use the built-in search functionality to find specific articles or topics:

```
https://www.informermoney.com/search?q=retirement+planning
```

### Subscribing to the Newsletter

Visit the homepage or blog and enter your email in the newsletter section to receive weekly financial insights.

### CMS & Content Authoring (Sanity Studio)

If you are a content author or editor, launch the local Sanity Studio:

```bash
cd studio
npm install
npm run dev
```

Access the studio at:

```
http://localhost:3333
```

### API Routes (if applicable)

```bash
# Fetch latest articles
GET /api/posts

# Fetch posts by category
GET /api/posts?category=investing

# Fetch a single post
GET /api/posts/:slug
```

---

## 📂 Content Categories

Informer Money currently covers the following eight editorial categories:

| Category                           | Description                                                          |
|------------------------------------|----------------------------------------------------------------------|
| 💹 **Investing**                   | Stocks, IRAs, ETFs, beginner guides, and retirement strategies       |
| 🏦 **Banking & Credit**            | Credit cards, loans, savings accounts, and credit score improvement  |
| 🧾 **Taxes & Insurance**           | Tax deductions, filing guides, life insurance comparisons            |
| 🏠 **Real Estate**                 | Home buying, mortgages, rental income, and market analysis           |
| 💼 **Business & Entrepreneurship** | Business plans, small business taxes, startup guides                 |
| 💵 **Personal Finance**            | Budgeting, saving, debt payoff, and financial planning               |
| 🏛️ **Economy & Policy**            | Fed decisions, inflation, interest rates, and macroeconomic analysis |
| 👷 **Work & Income**               | Salary negotiation, side hustles, career finance, and income growth  |

---

## 🤝 Contributing

We welcome contributions from developers, designers, financial writers, and educators alike. Please read the full guidelines below before submitting.

### How to Contribute

1. **Fork the repository:**

   ```bash
   git fork https://github.com/Informer-Money.git
   ```

2. **Create a feature branch:**

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes** and ensure they follow the project code style.

4. **Commit your changes** using a clear and descriptive message:

   ```bash
   git commit -m "feat: add dark mode toggle to article layout"
   ```

5. **Push to your branch:**

   ```bash
   git push origin feature/your-feature-name
   ```

6. **Open a Pull Request** against the `main` branch. Include a summary of your changes and link any related issues.

### Contribution Guidelines

- Follow the [Conventional Commits](https://www.conventionalcommits.org/) specification for commit messages.
- Ensure all new code passes linting: `npm run lint`.
- Do not submit pull requests that include copyrighted financial content without proper attribution.
- For large features or structural changes, open an issue first to discuss the approach.
- Content contributions (articles, guides) must comply with Informer Money's [Editorial Guidelines](https://www.informermoney.com/about#guidelines).

### Reporting Bugs

Please open a [GitHub Issue](https://github.com/Informer-Money) with:

- A clear title and description of the bug
- Steps to reproduce the issue
- Expected vs. actual behavior
- Browser and OS version (for UI bugs)

---

## 📄 License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2026 Informer Money

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

> **Note:** Editorial content (articles, guides, and associated media) published on [informermoney.com](https://www.informermoney.com/) is © 2026 Informer Money and is **not** covered by this license. All rights to editorial content are reserved.

---

## 📬 Contact

For inquiries related to the platform, editorial partnerships, or technical issues, please use the following channels:

| Channel             | Details                                                                 |
|---------------------|-------------------------------------------------------------------------|
| 🌐 **Website**      | [www.informermoney.com](https://www.informermoney.com/)                 |
| 📩 **Contact Form** | [informermoney.com/contact](https://www.informermoney.com/contact)      |
| 📰 **About & Team** | [informermoney.com/about](https://www.informermoney.com/about)          |
| 📋 **Editorial**    | [Editorial Guidelines](https://www.informermoney.com/about#guidelines)  |
| 🐛 **Bug Reports**  | [GitHub Issues](https://github.com/Informer-Money)      |
| 📬 **Newsletter**   | [Subscribe](https://www.informermoney.com/about#newsletter)             |

---

<p align="center">
  Made with ❤️ by the <a href="https://www.informermoney.com/about#team">Informer Money Editorial Team</a><br/>
  <sub>Smart financial guidance for building wealth, managing money, and navigating today's economy.</sub>
</p>
