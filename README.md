# Engagement Party RSVP Website

A beautiful, responsive website for collecting RSVPs for your engagement party using HTML, CSS, JavaScript, and Google Forms.

## Features

- ✨ Modern, elegant design with romantic styling
- 📱 Fully responsive for all devices
- 🎨 Beautiful gradients and animations
- 📝 Embedded Google Form for RSVP collection
- ⏰ Countdown timer to RSVP deadline
- 🖼️ Gallery section for your story
- 📧 Contact information for alternative RSVP methods

## Setup Instructions

### 1. Create a Google Form

1. Go to [Google Forms](https://forms.google.com)
2. Click the "+" button to create a new form
3. Title your form "Engagement Party RSVP"
4. Add the following questions:

#### Required Questions:

- **Name** (Short answer, required)
- **Email** (Short answer, required)
- **Will you attend?** (Multiple choice: Yes/No/Maybe, required)
- **Number of guests** (Short answer, required)
- **Dietary restrictions** (Paragraph, optional)
- **Message for the couple** (Paragraph, optional)

### 2. Get Your Form Embed Code

1. In your Google Form, click the **Send** button
2. Click the **Embed** tab
3. Copy the iframe code that looks like this:
   ```html
   <iframe
     src="https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform?embedded=true"
     width="640"
     height="800"
     frameborder="0"
     marginheight="0"
     marginwidth="0"
     >Loading…</iframe
   >
   ```

### 3. Update the Website

1. Open `index.html` in a text editor
2. Find this line (around line 75):
   ```html
   <iframe src="https://docs.google.com/forms/d/e/YOUR_FORM_ID/viewform?embedded=true"
   ```
3. Replace `YOUR_FORM_ID` with the actual form ID from your Google Form URL
4. Save the file

### 4. Customize the Content

Edit the following in `index.html`:

- **Couple names**: Change "Sarah" and "Michael" to your names
- **Event details**: Update date, time, location, and other details
- **Contact email**: Change `rsvp@engagementparty.com` to your email
- **RSVP deadline**: Update the date in both HTML and JavaScript files

### 5. Customize Styling (Optional)

Edit `styles.css` to change:

- Colors (search for `#667eea` and `#764ba2` for the main gradient)
- Fonts (currently using Playfair Display and Montserrat)
- Layout and spacing

## File Structure

```
wedding-invite/
├── index.html          # Main website file
├── styles.css          # CSS styling
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## How to Deploy

### Option 1: GitHub Pages (Free)

1. Create a GitHub repository
2. Upload your files
3. Go to Settings > Pages
4. Select "Deploy from a branch"
5. Choose "main" branch
6. Your site will be available at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free)

1. Go to [Netlify](https://netlify.com)
2. Drag and drop your website folder
3. Your site will be deployed instantly

### Option 3: Local Testing

1. Open `index.html` in your web browser
2. The website will work locally, but the Google Form needs to be properly configured

## Google Forms Features

- **Automatic responses**: Google Forms automatically collects responses in a spreadsheet
- **Email notifications**: Set up email notifications for new responses
- **Response summary**: View charts and summaries of responses
- **Export data**: Download responses as CSV or Excel files

## Customization Tips

### Adding Real Photos

Replace the placeholder gallery items with real photos:

```html
<div class="gallery-item">
  <img src="path/to/your/photo.jpg" alt="Description" />
</div>
```

### Changing Colors

Update the CSS variables in `styles.css`:

```css
:root {
  --primary-color: #667eea;
  --secondary-color: #764ba2;
  --accent-color: #ffd700;
}
```

### Adding More Sections

You can easily add new sections by following the existing pattern in the HTML file.

## Troubleshooting

### Form Not Loading

- Check that your Google Form is published and public
- Verify the form ID in the iframe URL
- Make sure you're not blocking iframes in your browser

### Styling Issues

- Clear your browser cache
- Check that all CSS and JavaScript files are in the same directory
- Verify that the file paths in your HTML are correct

### Mobile Responsiveness

- Test on different devices and screen sizes
- Use browser developer tools to simulate mobile devices

## Support

If you need help customizing your website or setting up Google Forms, feel free to:

- Check the Google Forms documentation
- Use browser developer tools to debug issues
- Test on different browsers and devices

## License

This project is open source and available under the MIT License.

---

**Happy planning! 🎉**
