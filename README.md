# Diana Olifirova Portfolio Clone

A modern, responsive portfolio website showcasing cinematography work with full-screen video backgrounds and scroll-snap navigation. Built with HTML, Tailwind CSS, and video integration.

## Features

- **Full-screen video backgrounds** with grayscale filters that animate on hover
- **Scroll-snap navigation** for smooth section transitions
- **Mix-blend-mode headers** that adapt to background content
- **YouTube video integration** for project previews
- **Responsive design** optimized for all devices
- **Loading states** for video content

## Project Structure

```
.
├── README.md
├── index.html                    # Main portfolio page with video backgrounds
└── projects/                     # Individual project pages
    ├── bridgerton-s3---netflix.html
    ├── nike-football---iconoclast.html
    └── twiggy.html
```

## Setup

1. Clone or download the repository
2. No build process required - files can be served directly
3. Open with a local server:
   ```bash
   python3 -m http.server 8000
   ```
4. Visit `http://localhost:8000` in your browser

## Adding Your Own Videos

### Background Videos (MP4 format)

Replace the placeholder video URLs in `index.html`:

```html
<!-- Bridgerton Section -->
<source src="YOUR_BRIDGERTON_VIDEO_URL.mp4" type="video/mp4">

<!-- Nike Football Section -->
<source src="YOUR_NIKE_VIDEO_URL.mp4" type="video/mp4">

<!-- Twiggy Section -->
<source src="YOUR_TWIGGY_VIDEO_URL.mp4" type="video/mp4">
```

**Video Requirements:**
- Format: MP4 (H.264 codec recommended)
- Resolution: 1920x1080 or higher
- Duration: 10-30 seconds (will loop automatically)
- File size: Keep under 50MB for web performance

### YouTube Preview Videos

Replace the YouTube video IDs in the Preview buttons:

```javascript
// In index.html, find these lines and replace the video IDs:
openModal('YOUR_BRIDGERTON_VIDEO_ID')  // Replace with actual YouTube video ID
openModal('YOUR_NIKE_VIDEO_ID')        // Replace with actual YouTube video ID
openModal('YOUR_TWIGGY_VIDEO_ID')      // Replace with actual YouTube video ID
```

**How to get YouTube video ID:**
- From URL `https://www.youtube.com/watch?v=ABC123xyz`, the ID is `ABC123xyz`
- From URL `https://youtu.be/ABC123xyz`, the ID is `ABC123xyz`

### Project Detail Pages

In each project page (e.g., `projects/bridgerton-s3---netflix.html`), replace:

```html
<!-- Main video embed -->
<iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID" ...></iframe>

<!-- Background video -->
<source src="YOUR_BACKGROUND_VIDEO_URL.mp4" type="video/mp4">

<!-- Additional video clips -->
<source src="YOUR_CLIP_1_URL.mp4" type="video/mp4">
<source src="YOUR_CLIP_2_URL.mp4" type="video/mp4">
<source src="YOUR_CLIP_3_URL.mp4" type="video/mp4">
```

## Design Features

### Video Effects
- **Grayscale filter** applied by default
- **Color restoration** on hover
- **Smooth transitions** between states
- **Auto-play and loop** for background videos

### Navigation
- **Scroll-snap** for precise section alignment
- **Mix-blend-mode** headers that invert based on background
- **Smooth scrolling** between sections
- **Keyboard navigation** (ESC to close modals)

### Responsive Design
- **Mobile-first** approach
- **Touch-friendly** interactions
- **Optimized video loading** for different devices

## Customization

### Colors and Styling
- Modify Tailwind classes in the HTML files
- Update CSS custom properties for consistent theming
- Adjust video filters and transitions in the `<style>` sections

### Content
- Update project titles, directors, and descriptions
- Modify technical specifications
- Replace placeholder images with actual project stills

### Performance Optimization
- Compress videos before uploading
- Use appropriate video formats for different browsers
- Consider lazy loading for additional content

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

**Note:** Video autoplay policies vary by browser. Some browsers may require user interaction before playing videos.

## Deployment

### Static Hosting
- GitHub Pages
- Netlify
- Vercel
- Any static file server

### Video Hosting
- Upload videos to a CDN or cloud storage
- Ensure CORS headers are properly configured
- Consider using video streaming services for large files

## Credits

- **Fonts:** Google Fonts (Poppins)
- **CSS Framework:** Tailwind CSS
- **Placeholder Videos:** Mixkit (for demonstration)
- **Original Design:** Inspired by Diana Olifirova's portfolio

## License

This is a clone project for educational purposes. Original design credits go to Diana Olifirova.
