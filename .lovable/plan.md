

# Will You Be My Valentine, Fenina? - Implementation Plan

## Overview
A romantic, interactive Valentine's website featuring a Rose Gold and Burgundy theme with magical animations, a photo gallery, love letter section, and hidden surprises throughout.

---

## What Will Be Built

### Page Structure
1. **Welcome Page** (/) - Hero with Fenina's name and path selection
2. **Our Story Page** (/our-story) - Photo gallery and love letter
3. **Valentine Question Page** (/valentine) - The big proposal moment

---

## Design System

### Color Palette
- **Burgundy**: Deep romantic red for primary elements
- **Rose Gold**: Warm metallic pink for accents and highlights
- **Cream**: Soft background tones
- **White/Pink**: Text and subtle accents

### Typography
- Elegant script fonts for headers (via Google Fonts)
- Clean, readable body text

---

## Page Details

### Page 1: Welcome
- Full-screen hero with "For Fenina" in elegant typography
- Floating hearts animation in background
- Sparkle particle effects
- Two beautiful buttons:
  - "Our Love Story" - navigates to /our-story
  - "A Special Question" - navigates to /valentine
- Subtle hint about hidden surprises

### Page 2: Our Story (/our-story)
- **Photo Gallery**: Grid of 6 placeholder images with captions
- **Love Letter**: Scrolling romantic letter section with placeholder text
- **Hidden Surprises**: 
  - Hover effects reveal secret love notes
  - Clickable elements unlock "Memory Explorer" achievement

### Page 3: Valentine Question (/valentine)
- Animated build-up sequence
- "Will you be my Valentine, Fenina?" with heart animations
- Interactive Yes button with celebratory effects
- Confetti and hearts explosion on acceptance
- "You Said Yes!" achievement unlocked

---

## Special Features

### Animations
- Floating hearts component (continuous background animation)
- Sparkle effects on hover
- Smooth page transitions
- Heart burst celebrations

### Hidden Surprises System
- 5-7 hidden "I love you" messages across all pages
- Secret love notes appearing on specific interactions
- Achievement badges tracking:
  - "Memory Explorer" - found on Our Story page
  - "You Said Yes!" - unlocked after accepting
  - "Secret Hunter" - finding hidden messages
- Progress counter showing surprises discovered

---

## Files to Create

### Core Components
- `src/components/FloatingHearts.tsx` - Background heart animation
- `src/components/Sparkles.tsx` - Sparkle effect component
- `src/components/HiddenMessage.tsx` - Reveals secret messages on interaction
- `src/components/AchievementBadge.tsx` - Achievement notifications
- `src/components/Confetti.tsx` - Celebration effects
- `src/components/PhotoGallery.tsx` - Image grid with captions
- `src/components/LoveLetter.tsx` - Styled letter component

### Pages
- `src/pages/Index.tsx` - Welcome page (update existing)
- `src/pages/OurStory.tsx` - Photo gallery and love letter
- `src/pages/Valentine.tsx` - The proposal page

### Hooks & Context
- `src/hooks/useSecrets.tsx` - Track discovered surprises
- `src/context/SecretsContext.tsx` - Global state for achievements

### Styles
- Update `src/index.css` - Add Valentine theme colors and animations
- Update `tailwind.config.ts` - Add custom colors and keyframes

---

## What You'll Personalize Later
- Replace placeholder photos with your real pictures
- Customize the love letter text
- Add your own memory captions
- Include specific dates or inside jokes

---

## Technical Notes
- All animations use CSS keyframes and Tailwind for performance
- Responsive design works on mobile and desktop
- State persisted in localStorage so she can return and see her achievements
- Smooth transitions between pages using React Router

