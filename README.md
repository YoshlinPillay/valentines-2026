# 💕 Valentine's Day Website for Your Special Someone

A playful, animated Valentine's Day website with an impossible-to-click "No" button!

## Features

- ✨ Animated, pulsing question text with shimmer effects
- 📸 Circular photo frame with floating animation
- 🎯 "No" button that runs away when you try to click it
- ❤️ "Are you sure?" confirmation with teasing message
- 💖 Heart explosion animation when confirmed
- 🎉 "YAAAS" celebration followed by photo slideshow
- 🐱 Final reveal with your family (including cat!)

## Setup Instructions

### 1. Add Your Images

Replace the placeholder images in the `images/` folder:

| File | Description | Recommended Size |
|------|-------------|------------------|
| `her.jpg` | Photo of your wife | Square, at least 500x500px |
| `us.jpg` | Photo of you two together | Any aspect ratio, 800px+ wide |
| `us-with-cat.jpg` | Photo of you both with your cat | Any aspect ratio, 800px+ wide |
| `yaas.gif` | A fun "YAAAS" reaction GIF | Any size (will be resized) |

**Finding a YAAAS GIF:**
- Go to [GIPHY](https://giphy.com/search/yaaas)
- Or [Tenor](https://tenor.com/search/yaas-gifs)
- Download and save as `yaas.gif`

### 2. Deploy to GitHub Pages (Free)

1. Create a new GitHub repository (e.g., `valentine-for-[wife-name]`)
2. Upload all files:
   ```
   index.html
   images/
     ├── her.jpg
     ├── us.jpg
     ├── us-with-cat.jpg
     └── yaas.gif
   ```
3. Go to **Settings** → **Pages**
4. Under "Source", select **main** branch
5. Click **Save**
6. Your site will be live at: `https://[your-username].github.io/[repo-name]/`

### 3. Deploy to Netlify (Free Alternative)

1. Go to [Netlify](https://app.netlify.com/)
2. Sign up/Login
3. Drag and drop your `valentine` folder onto the Netlify dashboard
4. Done! You'll get a random URL like `random-name-123.netlify.app`
5. (Optional) Click "Site settings" to customize the URL

## Customization

### Change Colors
Edit the CSS variables at the top of `index.html`:

```css
:root {
    --rose: #e63946;        /* Main red/pink */
    --blush: #f8b4b4;       /* Light pink */
    --cream: #fff5f5;       /* Background cream */
    --deep-rose: #c1121f;   /* Dark red for text */
    --gold: #d4a373;        /* Gold accents */
    --soft-pink: #ffd6e0;   /* Soft pink gradient */
}
```

### Change the Question
Find this line and edit the text:
```html
<h1 class="question">Will You Be My Valentine?</h1>
```

### Change Final Messages
Look for these in the JavaScript section:
```javascript
<p class="final-message">Forever & Always 💕</p>
<p class="final-message">Our Little Family 🐱💕</p>
finalMsg.innerHTML = 'I Love You! ❤️';
```

### Adjust Timing
The photo slideshow timing is in the `showYaaas()` function:
- YAAAS gif shows for 3 seconds
- "Us" photo shows for 4 seconds
- Then transitions to photo with cat

## Browser Support

Works best in modern browsers:
- ✅ Chrome
- ✅ Firefox
- ✅ Safari
- ✅ Edge

## Made with 💕

Happy Valentine's Day! 

---

*Tip: For extra romantic points, send the link with a sweet message!*
