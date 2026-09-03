# Bharat Bhushan Interiors

[![Live Website](https://img.shields.io/badge/Live%20Website-bharatbhushancompany.com-0F9D58?style=for-the-badge&logo=googlechrome&logoColor=white)](https://bharatbhushancompany.com/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)
[![Cloudflare Workers](https://img.shields.io/badge/Cloudflare%20Workers-F38020?style=for-the-badge&logo=cloudflareworkers&logoColor=white)](https://workers.cloudflare.com/)
[![EmailJS](https://img.shields.io/badge/EmailJS-0A0A0A?style=for-the-badge&logo=mailgun&logoColor=white)](https://www.emailjs.com/)

> A fast, responsive, and production-deployed website for **Bharat Bhushan & Company**, presenting commercial furniture, interior-design services, completed spaces, and an online enquiry experience.

**Live website:** [https://bharatbhushancompany.com/](https://bharatbhushancompany.com/)

---

## Dashboard and deployment

![Cloudflare deployment dashboard](dashboard.png)

The website is live behind Cloudflare and served by the `interior` Worker route for `bharatbhushancompany.com/*`. Cloudflare provides DNS proxying, HTTPS/TLS, caching, and edge delivery for the production website.

## About the project

Bharat Bhushan Interiors is a client-focused business website built to make it easy for visitors to explore interior-design ideas, furniture collections, company information, project galleries, and contact options. The site is designed for a clean experience across desktop and mobile devices.

The source repository is kept private to protect project implementation, client assets, and deployment configuration. This document provides a public overview of the finished product.

## Highlights

- Responsive user interface for mobile, tablet, and desktop screens
- Home page with hero slideshow, featured collections, and service highlights
- Product catalogue covering office furniture and interior solutions
- Dynamic product-detail pages powered by URL parameters
- Residential design-idea galleries for living rooms, kitchens, bedrooms, bathrooms, wardrobes, and more
- Client and completed-project showcase
- Contact page with location details and embedded Google Map
- Online enquiry form with client-side validation and EmailJS delivery
- Local Font Awesome assets and image gallery optimisation
- Production deployment through Cloudflare with custom-domain HTTPS

## Technology stack

| Area | Technology |
| --- | --- |
| Markup | HTML5 |
| Styling | CSS3 |
| Programming language | Vanilla JavaScript |
| Hosting and edge delivery | Cloudflare Workers |
| Form and email delivery | EmailJS |
| Icons | Font Awesome Free |
| Typography | Google Fonts — Poppins |
| Source control | Git and GitHub |

## Architecture

```text
Visitor browser
    │
    ├── Cloudflare DNS, HTTPS, caching, and edge delivery
    │
    └── Cloudflare Worker: interior
            │
            ├── Static HTML, CSS, JavaScript, images, and fonts
            └── EmailJS enquiry submission
```

The application is intentionally lightweight. It does not require a traditional backend server, database, framework, or build pipeline for normal site delivery.

## Core pages

| Page | Purpose |
| --- | --- |
| Home | Introduces the company, key services, products, and design work |
| About Us | Communicates the company story, services, and process |
| Our Products | Presents furniture and workplace-interior categories |
| Product Details | Shows category-specific descriptions, galleries, features, and related products |
| Design Ideas | Displays residential interior inspiration |
| Our Clients | Highlights client work and completed spaces |
| Contact Us | Shares contact details, location, and Google Map |
| Send Enquiry | Collects a visitor's contact details and requirements |

## Enquiry workflow

1. A visitor completes the consultation form with their name, email address, mobile number, and requirement.
2. Browser-side validation checks the required fields and Indian mobile-number format.
3. EmailJS submits the enquiry to the configured business email service.
4. The visitor receives a clear confirmation message after successful submission.

## Security and production practices

- HTTPS/TLS is provided through Cloudflare for encrypted visitor connections.
- Security-oriented response headers and caching rules are maintained in the deployment configuration.
- The site uses local image and Font Awesome assets where possible.
- No private EmailJS key, mailbox password, Cloudflare API token, or other server secret is included in this public project overview.
- The EmailJS public browser key is intentionally separate from private service credentials; origin restrictions and anti-spam controls should remain configured in the EmailJS dashboard.

## Local development

For authorised source-code access, the site can be run without installing dependencies:

```powershell
cd Interia
python -m http.server 8000
```

Then open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in a browser. Stop the server with `Ctrl+C`.

## Deployment checklist

- Confirm the `bharatbhushancompany.com/*` Worker route is active.
- Verify HTTPS is enabled and the custom domain resolves correctly.
- Test each main navigation link on desktop and mobile.
- Submit a real enquiry and confirm delivery through EmailJS.
- Confirm Cloudflare caching and response-header rules are present after release.

---

## Developer

[![GitHub](https://img.shields.io/badge/GitHub-Ravishyamsingh-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ravishyamsingh)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit%20Website-6C63FF?style=for-the-badge&logo=googlechrome&logoColor=white)](https://ravishyamportfolio.netlify.app/)

**Ravi Shyam Singh**  
*Software Engineer*

Ravi Shyam Singh is a Software Engineer focused on building practical, polished, and user-centred web experiences. His work spans responsive frontend development, full-stack applications, AI-powered collaboration tools, and production deployments.

- GitHub: [github.com/Ravishyamsingh](https://github.com/Ravishyamsingh)
- Portfolio: [ravishyamportfolio.netlify.app](https://ravishyamportfolio.netlify.app/)

### Visit my other projects

1. Java Learning Project: [java-course.vercel.app](https://java-course.vercel.app/)
2. SyncSpace — Multi-Agent AI Workspace: [syncspace-neon.vercel.app](https://syncspace-neon.vercel.app/)
3. Smart Gym Access & Management Platform: [olympia-fitness.netlify.app](https://olympia-fitness.netlify.app/)


