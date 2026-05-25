# Piano Lessons with Minnie Website

Simple static website for Piano Lessons with Minnie, a personal children’s piano lesson business centered around Minnie.

## Folder Structure

```text
.
├── index.html
├── lessons.html
├── about.html
├── contact.html
├── styles.css
└── assets/
    └── images/
        ├── contact-placeholder.svg
        ├── lesson-room-placeholder.svg
        ├── minnie-at-grand-piano.jpg
        ├── minnie-placeholder.svg
        ├── minnie-with-students.jpg
        ├── minnie-with-young-student.jpg
        ├── piano-lesson-placeholder.svg
        ├── piano-lesson-student.jpg
        └── student-recital.jpg
```

## Updating Text

- Home page text: edit `index.html`
- About page text: edit `about.html`
- Lessons page text and FAQ: edit `lessons.html`
- Contact page text and form fields: edit `contact.html`
- Phone and footer details appear on all pages.

Search for the current value, such as `+1 (646) 288-8821`, and update it everywhere it appears.

## Updating Images

Photos and placeholder images live in `assets/images/`.

To replace one:

1. Add the new image to `assets/images/`.
2. In the related HTML file, update the `src` value.
3. Update the `alt` text so it describes the real image.

Example:

```html
<img src="assets/images/minnie.jpg" alt="Minnie smiling beside a piano">
```

## Contact Form

The form in `contact.html` includes Netlify form attributes:

```html
<form name="lesson-inquiry" method="post" data-netlify="true">
```

After deploying on Netlify, form submissions should appear in the Netlify dashboard under Forms.

## Deploying to Netlify

1. Create a Netlify account or sign in.
2. Choose **Add new site**.
3. Upload this folder, or connect a GitHub repository containing these files.
4. Build settings:
   - Build command: leave blank
   - Publish directory: `.`
5. Deploy the site.
6. After deployment, test the contact form and update the site URL in any future structured data if needed.

## SEO Notes

Each page includes its own SEO title and description. The copy naturally includes phrases such as:

- children’s piano lessons
- private piano lessons
- in-home piano lessons
- Manhattan piano lessons
- Queens piano lessons
- beginner piano lessons
- ABRSM exam preparation
- Trinity exam preparation

JSON-LD structured data is included in each page to help search engines understand the business and lesson services.
