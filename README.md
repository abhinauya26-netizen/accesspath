# AccessPath 🦯♿

## AI-Powered Accessibility-Aware Campus Navigator

AccessPath is a web-based campus navigation system designed to help students and visitors find routes that are not only short, but also suitable for their accessibility needs.

Instead of simply choosing the shortest path, AccessPath uses accessibility profiles and a Dijkstra-based routing engine to recommend safer and more accessible routes.

## ✨ Features

- 🧭 Accessibility-aware campus navigation
- ♿ Wheelchair-friendly routing
- 🦯 Blind / Low Vision text and audio guidance
- 🧓 Elderly accessibility profile
- 🩹 Temporary Injury profile
- 👶 Stroller profile
- 🗺️ Interactive campus SVG map
- 📍 Shortest route vs. recommended accessible route
- 🤖 AI-assisted accessibility issue reporting
- 📸 Report campus accessibility problems
- 📊 Admin dashboard for accessibility issues
- 💾 Local storage for demo data
- 🔊 Browser speech synthesis for audio guidance
- ♿ Accessibility-focused UI and ARIA support

## 🧠 How It Works

AccessPath calculates two routes:

1. **Shortest Distance Route**
2. **Accessibility-Optimized Route**

The accessibility route applies profile-specific rules, penalties, and hard exclusions.

For example, for a wheelchair user:

- Stairs are excluded
- Slopes above 8% are excluded
- Narrow paths are penalized
- Rough surfaces are penalized
- Ramps and elevators are preferred

This allows AccessPath to explain why a longer route may be better than the shortest route.

## 🤖 AI-Assisted Reporting

Users can report accessibility problems such as:

- Blocked ramps
- Broken elevators
- Uneven surfaces
- Obstructions
- Accessibility hazards

The system analyzes the report and provides:

- Issue type
- Severity
- Confidence
- Accessibility impact
- Recommended action
- Affected accessibility profiles
- Human-review recommendation

The project includes a deterministic demo fallback when an on-device vision model is unavailable.

## 🛠️ Technology Stack

- React
- Vite
- JavaScript
- CSS
- Inline SVG
- Browser Speech Synthesis API
- LocalStorage
- Dijkstra's algorithm

No external APIs or login systems are required for the demo.

## 🚀 Running Locally

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/accesspath.git
