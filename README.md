# Startup Static Website

This is a responsive static website designed for a startup to promote its products and services. It includes six well-structured web pages: Home, About Us, Services, Portfolio, Blog, and Contact Us. The site was built using HTML and CSS with a mobile-first and accessible design approach.

---

## 🌐 Website Pages

- **Home** – Engaging hero section with call-to-action.  
- **About Us** – Information about the team and company mission.  
- **Services** – A list of services offered, shown in card layout.  
- **Portfolio** – Displays sample work in a grid with hover overlays.  
- **Blog** – Article previews in a grid format.  
- **Contact Us** – Basic contact information and a contact form (static placeholder).

Each page includes a consistent navigation bar and footer for a unified user experience.

---

## 🛠️ Built With

- **HTML5**  
- **CSS3**  
- **Flexbox and Grid Layouts**  
- **Responsive Design via Media Queries**  
- **Custom Animations and Transitions**

---

## 🔄 CI/CD & DevOps Focus

The primary objective of this project was to **learn and implement modern CI/CD workflows**:

1. **Git Flow**  
   - Feature branches for each page: `feature/home`, `feature/aboutus`, etc.  
   - `develop`, `release/*`, and `production` branches with branch-protection rules.

2. **GitHub Actions**  
   - **Development Workflow**: Lint, build and deploy on push/PR to `develop`.  
   - **Staging Workflow**: Trigger on creation of `release/*` branch, deploy to staging environment.  
   - **Production Workflow**: Trigger on merge to `production`, deploy to live site.

3. **Environments**  
   - `development-env`, `staging-env`, and `production-env` configured in GitHub.  
   - Protected branches require status checks, PR reviews, and successful CI passes.

Feel free to extend the workflows with additional steps—unit tests, performance audits, or automated UI tests.

---

## 📁 Project Structure

project-root/
│
├── index.html
├── aboutus.html
├── services.html
├── portfolio.html
├── blog.html
├── contact.html
│
├── styles/
│ ├── homepage.css
│ ├── aboutus.css
│ ├── services.css
│ ├── portfolio.css
│ ├── blog.css
│ └── contact.css
│
├── .github/
│ └── workflows/
│ ├── dev-deployment.yml
│ ├── staging-deployment.yml
│ └── prod-deployment.yml
│
├── assets/
│ ├── images/
│ └── icons/
│
└── README.md
