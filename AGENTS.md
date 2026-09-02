# AI Agent Guide for my-portfolio

## Project Overview
Personal portfolio website for Dickie — a statistics and programming student focused on AI-certified automation systems. This is a **static HTML/CSS/JS site** with no build tooling or npm dependencies.

## Key Facts for Agents

### Directory Structure
```
docs/
  ├── index.html          # Main entry point
  ├── script.js           # Vanilla JS (scroll-reveal, no dependencies)
  └── css/
      └── style.css       # All styling + CSS custom properties
```

### Development & Deployment
- **Local server**: `python3 -m http.server 8000` then visit `http://localhost:8000/docs`
- **Deployment**: Files in `/docs/` are ready for GitHub Pages or any static host
- **No dependencies**: This is vanilla HTML/CSS/JS — no npm, no build step

### Design System
**CSS Custom Properties** (defined in `:root`):
- **Colors**: 
  - `--bg`: `#0B0F14` (dark background)
  - `--accent`: `#E3B341` (signal amber — primary highlight)
  - `--accent-2`: `#4FD1C5` (data teal — secondary highlight)
  - `--text`: `#E7ECEF` (light text)
  - `--muted`: `#8B98A5` (muted text)
- **Typography**:
  - `--display`: Space Grotesk (headings)
  - `--body`: IBM Plex Sans (body text)
  - `--mono`: IBM Plex Mono (code/terminal style)
- **Other**: `--panel`, `--panel-2`, `--line` for section backgrounds and borders

### Code Patterns
1. **Scroll Reveal Animation** (`script.js`):
   - Uses `IntersectionObserver` to fade-in elements on scroll
   - Respects `prefers-reduced-motion` for accessibility
   - Targets: `.stage`, `.skill-card`, `.project`, `.stat`

2. **Styling Approach**:
   - Mobile-first responsive design
   - CSS variables for consistent theming
   - Minimal reset (box-sizing, margin/padding)
   - Smooth scroll behavior enabled

3. **HTML Structure**:
   - Semantic sections: hero, work, skills, process, contact
   - Navigation bar with smooth scroll links
   - Profile image reference at `profile.jpg/profile.jpg` (verify path)

### Common Tasks for Agents
- **Update content**: Edit `.html` to add/modify sections
- **Change colors**: Update `:root` CSS variables
- **Fix responsive issues**: Modify CSS media queries
- **Add animations**: Extend `.js` scroll-reveal logic or add CSS transitions
- **Update fonts**: Change Google Fonts link in `<head>`

### Accessibility
- All animations respect `prefers-reduced-motion`
- Semantic HTML structure
- Proper heading hierarchy
- Image alt text

### Known Issues to Watch
- Profile image path: `profile.jpg/profile.jpg` may need correction
- Ensure all external font links remain valid
- Test smooth scroll on all browsers

## Quick Commands
```bash
# Start local dev server
cd /workspaces/my-portfolio && python3 -m http.server 8000

# View in browser
open http://localhost:8000/docs
```
