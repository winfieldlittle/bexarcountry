# BexarCountry.com

A clean, performant static website for BexarCountry.com, hosted on Porkbun. The site features a custom contact/email form that securely submits data to a Google Sheet via Google Apps Script, enabling seamless form handling without a traditional backend server.

## Project Overview

**BexarCountry.com** is a fully static HTML/CSS/JavaScript website designed for speed, reliability, and simplicity. By leveraging static hosting on Porkbun and Google Apps Script as a lightweight backend, the project demonstrates an elegant serverless approach to handling form submissions while maintaining full control over the frontend.

### Key Features

- **Static-first architecture** – Fast loading times, excellent SEO, and high security
- **Custom contact form** with client-side validation
- **Serverless form processing** using Google Apps Script + Google Sheets
- **No backend server required** – Reduced cost, maintenance, and attack surface
- **Porkbun hosting** with custom domain configuration
- **Responsive, modern design** optimized for all devices

## Architecture

This project intentionally uses a **static + serverless** stack:

- **Frontend**: Pure HTML, CSS, and vanilla JavaScript (no heavy frameworks)
- **Hosting**: Porkbun static hosting
- **Form Handling**: Google Apps Script (Web App) → Google Sheets
- **Data Storage**: Google Spreadsheet (acts as a simple, accessible database)

This architecture provides an excellent balance between simplicity and functionality, making it ideal for small business sites, portfolios, and landing pages.

## Form Submission Flow

1. User submits the form on the website
2. JavaScript validates input and sends data via `fetch()` to the Google Apps Script Web App
3. Apps Script receives the POST request, validates it, and appends the data to a Google Sheet
4. Optional: Confirmation email or success message returned to the user

## Repository Structure
