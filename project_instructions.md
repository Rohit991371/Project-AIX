# Project Instructions: Colorful Animated Calculator

## 1. Project Overview
The goal of this project is to build a modern, simple, vibrant, and interactive web-based calculator. The application must feature colorful visual themes, smooth animations on button presses and display updates, responsive layout design, and full calculator functionality.

---

## 2. Technical Stack & Requirements
- **Language/Framework:** HTML5, CSS3, JavaScript (Vanilla ES6+) or React (Single File Component).
- **Styling:** CSS3 (Flexbox/Grid, Animations, Keyframes, Transitions, CSS Variables) or Tailwind CSS.
- **Dependencies:** Keep dependencies minimal to ensure fast load times and clean code.

---

## 3. UI/UX & Design Directives

### Visual Style
- **Theme:** Vibrant, modern dark/light contrast or gradient themes (e.g., Neon Pop, Pastel Synthwave, or Soft Glassmorphism).
- **Color Palette:**
  - Background: Soft dark/light background gradient.
  - Number Buttons: Subtle pastels or deep tones with bright text.
  - Operator Buttons (`+`, `-`, `*`, `/`, `=`): Eye-catching gradient or neon accent colors (e.g., Vibrant Purple, Electric Blue, Bright Pink).
  - Special Buttons (`AC`, `+/-`, `%`): Distinct warning/secondary colors.

### Animations & Keyframes
- **Button Click Effect:** Active state scale effect (`transform: scale(0.95)`), smooth ripple or glow effect.
- **Display Updates:** Smooth keyframe animation (e.g., subtle fade or slide-in) whenever numbers or calculation results change.
- **Hover States:** Smooth micro-interactions, subtle vertical translation (`translateY(-2px)`), and elevated box-shadows.

---

## 4. Core Calculator Functionality
1. **Basic Operations:** Addition (`+`), Subtraction (`-`), Multiplication (`*`), Division (`/`).
2. **Unary Operations:** Clear/All Clear (`AC`), Toggle Sign (`+/-`), Percentage (`%`).
3. **Decimal Input:** Support for floating-point calculations without duplicating decimals.
4. **Keyboard Support:** Full mapping for keyboard numpad and arithmetic keys.
5. **Error Handling:** Gracefully handle division by zero (e.g., display "Cannot divide by 0" with a shake animation).

---

## 5. Delivery Instructions
- Build the calculator based on these specification guidelines.
- Strictly adhere to the instructions in `AI_LOGGING_INSTRUCTIONS.md` to track model usage, performance, and decision logs.