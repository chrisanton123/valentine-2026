# Project Cupid's Trap 💕

A playful Valentine's Day proposal website that makes it nearly impossible to say "No" through interactive physics, games, and emotional appeals.

## 🎯 Features

- **Magnetic "No" Button**: The "No" button smoothly evades the cursor using physics-based movement
- **Progressive Escalation**: Each click on "No" makes it more dramatic and grows the "Yes" button
- **Valentine's Integrity Check**: A slot machine mini-game that verifies your choice
- **Responsive Design**: Works beautifully on desktop and mobile devices
- **Romantic Aesthetics**: Custom fonts, gradients, floating hearts, and smooth animations

## 🚀 GitHub Pages Deployment

### Quick Setup (3 steps)

1. **Create a new GitHub repository**
   - Go to [GitHub](https://github.com/new)
   - Name it something like `valentine-proposal`
   - Make it public
   - Don't initialize with README (we have one)

2. **Upload the files**
   - Click "uploading an existing file"
   - Drag and drop `index.html` and `README.md`
   - Commit the files

3. **Enable GitHub Pages**
   - Go to your repository Settings
   - Scroll to "Pages" section
   - Under "Source", select `main` branch
   - Click Save
   - Your site will be live at: `https://yourusername.github.io/valentine-proposal/`

### Alternative: Command Line Setup

```bash
# Initialize git in your project folder
git init
git add .
git commit -m "Initial commit: Valentine's Day proposal site"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/valentine-proposal.git

# Push to GitHub
git branch -M main
git push -u origin main

# Then enable GitHub Pages in repository settings
```

## 🎨 Customization

You can easily customize the website:

- **Change the GIFs**: Replace the Giphy URLs in the `<img>` tags
  - Asking GIF (line ~206): Currently a pleading puppy
  - Success GIF (line ~218): Currently a celebration
  
- **Modify the messages**: Edit the `noButtonTexts` array (around line 313)

- **Adjust colors**: Change the CSS variables in `:root` (around line 17)

- **Change fonts**: Replace Google Fonts links in the `<head>` section

## 📱 How It Works

1. **Initial Screen**: Shows a romantic question with two buttons: "Yes" and "No"

2. **Magnetic No Button**: When you hover near "No", it moves away using vector mathematics

3. **Click Progression**: 
   - Each click on "No" changes its text to be more pleading
   - The "Yes" button grows larger with each attempt
   
4. **Slot Machine Game**: After 5 clicks, triggers a "Valentine's Integrity Check"
   - 3 RED (YES): Leads to broken heart state
   - 3 GREEN (NO): Button becomes disabled
   - Mixed: Try again!

5. **Final State**: Eventually, "No" becomes broken or disabled, leaving "Yes" as the only real option

6. **Success**: Clicking "Yes" shows a celebration with hearts raining down

## 🛠️ Technical Details

- **Pure HTML/CSS/JavaScript** - No frameworks needed
- **Responsive design** - Works on all screen sizes
- **Mobile-friendly** - Touch events handled differently than mouse
- **Smooth animations** - CSS transitions and keyframe animations
- **Physics-based movement** - Vector math for natural button movement

## 💡 Tips

- Test the site locally by opening `index.html` in your browser
- The "No" button is intentionally difficult but not impossible to click
- Mobile users will see the button jump around periodically instead of mouse-based movement
- All interactions are smooth and playful, not frustrating

## ❤️ Credits

Created with love for that special someone! Feel free to fork and customize for your own proposal.

---

**Good luck with your proposal! 🌹**
