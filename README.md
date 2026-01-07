🌀 Barrel Roll: Progressive Disclosure Template

A dynamic, step-by-step interactive interface designed for sequential content delivery. This "Barrel Roll" template uses a vertical sliding animation to transition between informational stages, guiding users through a logical flow of concepts or procedures.

🚀 Live Demo

Explore the Barrel Roll Interface Here

✨ Project Overview

The Barrel Roll activity is optimized for instructional content that must be viewed in a specific order. By utilizing a "Next Step" workflow and a central animated stage, it prevents information overload and ensures the user masters one concept before moving to the next.

Key Features

Vertical Transition Engine: Implements a custom CSS slide-in-up and slide-out-up animation suite to create a physical "scrolling" or "barrel" effect during content swaps.

Progress Tracking: A real-time indicator (e.g., "Step 1 of 3") keeps users oriented within the learning path.

Tick-Mark Validation: Custom-styled list items use a CSS-generated checkmark (✓) to reinforce completion and clarity within each step's explanation.

Branded Visual Identity:

Midnight Blue (#1f2a52): Used for the primary buttons and main titles.

Accent Teal (#00bec7): Powers the interactive hover states and the "Tick-Mark" icons.

Slate Grey (#abb5bf): Provides a neutral grounding for secondary text and structural borders.

Light Aqua (#d2f0f0): Sets a clean, professional background tone.

🛠️ Technical Implementation

Asynchronous DOM Swapping: Uses JavaScript's animationend events to cleanly remove old content layers and introduce new ones, preventing layout shifts.

Scrollable Content Stage: The central content container is fixed-height but includes overflow-y-auto, ensuring that even long descriptions remain accessible on smaller screens.

Vanilla JavaScript Logic: Manages the state of the currentIndex, toggling visibility for the "Next Step" and "Start Over" buttons based on the user's progress.

CSS Custom Properties: Defines a :root variable system for the brand palette, allowing for global color adjustments with a single line of code.

📂 Project Structure

Barrel_Roll_Activity/
├── index.html          # Core template, animation logic, and branded styles
├── previews/           # Automated UI capture assets
└── .github/workflows/  # CI/CD for catalog and preview synchronization


📖 Usage Instructions

Customizing Content

To update the steps, modify the stepsContent array in the <script> section. Each object supports a title and an explanation (which accepts HTML for lists and paragraphs).

Modifying Animations

The speed and physics of the transitions can be adjusted by editing the @keyframes and the .animate-slide-in-up classes within the <style> block.

📄 License

MIT License - Created for the accounts-eles ecosystem.
