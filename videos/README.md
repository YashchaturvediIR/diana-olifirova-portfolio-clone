# Video Setup Instructions

To add video backgrounds to the portfolio:

1. Download your video clips
2. Convert them to MP4 format (recommended specs below)
3. Place them in this directory
4. Update the video source paths in index.html

## Recommended Video Specifications

- Format: MP4 (H.264 codec)
- Resolution: 1920x1080 or higher
- Duration: 10-30 seconds (will loop automatically)
- File size: Keep under 10MB for optimal performance
- Aspect ratio: 16:9

## Expected Files

Replace these placeholder files with your actual videos:
- bridgerton-background.mp4
- nike-background.mp4
- twiggy-background.mp4

## HTML Update Example

In index.html, uncomment and update the video source:

```html
<video class="video-background" autoplay muted loop playsinline>
    <source src="/videos/bridgerton-background.mp4" type="video/mp4">
</video>
```

## Performance Tips

1. Compress videos to reduce file size
2. Consider using a CDN for video hosting
3. Provide a poster image for initial load
4. Keep videos short and loop seamlessly
