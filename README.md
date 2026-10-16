# Imran Pathan — Personal Portfolio

A React portfolio for **job/internship opportunities and freelance project enquiries**, based on the two supplied resumes. Warm neutral colours, orange accents, editorial typography and an animated code-to-cloud illustration.

## Run karne ke liye

Node.js **24 LTS** install karo, ZIP extract karo, phir `package.json` wale folder mein:

```powershell
npm.cmd ci
npm.cmd run dev
```

Browser mein **http://localhost:5174** kholo. Terminal khula rakho. Windows par `scripts/start.bat` double-click bhi kar sakte ho. macOS/Linux mein `npm ci` aur `npm run dev`.

**MongoDB ya backend setup ki zaroorat nahi hai.** This portfolio is a static React application. The contact form opens the visitor's email app with a prefilled enquiry; it does not send or store a message by itself. Direct email, copy-email and telephone links are included too.

## Features

- Animated hero with custom code/browser artwork, floating cards, orbital details and a scroll progress bar.
- Responsive mobile navigation with Escape support.
- Projects filtered by web development / DevOps, with keyboard-accessible native detail dialogs.
- Verified public GitHub links and the ShopWave live demo from its repository README.
- A real ShopWave screenshot sourced from the owner's repository. Other project covers are original illustrative diagrams, not application screenshots.
- Separate “Hire me” / “I have a project” contact paths.
- Both original full-stack and DevOps resume PDFs available for download.
- Services, skills, education and an honest early-career profile. AWS is clearly labelled as currently learning.
- Respects reduced-motion preferences; no scroll hijacking or custom cursor.

## Content change karna ho

- **`src/data.js`**: name, email, telephone, projects, GitHub links, skills and services.
- **`src/main.jsx`**: page copy and section layout.
- **`src/styles.css`**: design, colours, responsive layouts and animations.
- **`public/resumes/`**: replace the original resume PDFs while keeping filenames, or update the links in `main.jsx`.
- **`public/images/shopwave.jpg`**: project screenshot.

Expected BCA graduation is **2026**, as confirmed by the owner. A monogram is used because no personal photo was supplied. No client testimonials, employment history, certifications or invented performance metrics are included.

The original PDFs contain your contact information and will be publicly downloadable if you publish the site. Replace them with updated public versions if needed.

## Production build / deploy

```bash
npm run build
npm run preview
```

Production preview: **http://localhost:4174**. Built site: **`dist/`**.

For Vercel or Netlify, select the `portfolio` project directory, build command **`npm run build`**, output directory **`dist`**. If you upload only the contents of this portfolio folder into its own repository, choose that repository root instead. Uploading this ZIP does not deploy it automatically.

All assets except the Google Fonts are bundled locally. System font fallbacks are available when Google Fonts cannot load. The Render-hosted ShopWave demo may take time to wake up.

## Checks

```bash
npm test
npm run build
```

Tests cover safely encoded hiring/project email enquiries, project references and required downloadable assets. The project was also checked in shared Chromium on desktop/mobile for layout, filtering, navigation, dialogs, contact intent, clipboard feedback and accessibility.

## Design references

See [DESIGN-NOTES.md](DESIGN-NOTES.md) for research sources and how they informed this design.
