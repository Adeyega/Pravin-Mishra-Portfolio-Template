# DMI Portfolio Website (Static HTML/CSS)

This repository contains a clean, professional-looking **static portfolio website** used in **DevOps Micro Internship (DMI)** Week 1 to practice:
- Linux basics
- Nginx hosting
- Deployment proof / ownership
- Production-style checks

✅ Students deploy this website on an Ubuntu VM using Nginx and keep it live for 24 hours.

---

## Who is this for?
- DMI students (beginner → intermediate)
- Anyone learning how to host a static site with Nginx on Linux

---

## What you will build
A portfolio-style website hosted on:
- **Ubuntu VM**
- **Nginx**
- Accessible via: `http://<public-ip>`

---

## Mandatory Ownership Proof (DMI Rule)
Before you deploy, you MUST edit the footer and add your details:

Original:

```html
<p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
```

Add this line (example):

```html
<p><strong>Deployed by:</strong> DMI Cohort 2 | Rahul Sharma | Group 4 | Week 1 | 16-01-2026</p>
```
#### Footer Implementation

#### Footer Requirement

The footer was updated to display:

The website/portfolio name

Copyright text

The current year, generated dynamically so it updates automatically every year without manual changes

This ensures the site always looks up to date and professional.

How the Date Is Generated

The year in the footer is generated using JavaScript.
Instead of hard-coding a year (e.g. 2024), JavaScript retrieves the current year from the user’s system date and inserts it into the footer when the page loads.

This approach:

Prevents outdated copyright years

Requires no future manual updates

Follows best practices for modern web development

### Code Snippet

#### Footer HTML
```html
<footer>
  <p>
    © <span id="year"></span> Adegboyega Ogunsemoyin. All rights reserved.
  </p>
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>



✅ This proof must be visible in your browser screenshot submission.