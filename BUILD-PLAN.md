
Step 1 — Add the toggle button to the navbar
- Add a <button id="dark-mode-toggle"> with a ☀/🌙 icon to the <header> in all 4 HTML files
No JS or CSS yet — just the HTML element
Test: button appears in the navbar on every page

Step 2 — Define dark mode colors in styles.css
- Add a body.dark-mode { ... } block that overrides your existing CSS variables
No JavaScript yet — you can test by manually adding class="dark-mode" to <body> in your browser dev tools
Test: page looks correct in dark mode when class is manually toggled

Step 3 — Wire up the toggle button (JavaScript)
- Small <script> block: clicking the button adds/removes .dark-mode on <body>
Test: clicking the button switches the page live (resets on reload)

Step 4 — Persist preference with localStorage
- On load: check localStorage and apply dark mode if it was saved
On toggle: save or clear the preference
Test: reload the page → your preference sticks

Step 5 — Copy the script to all 4 pages
- The same script block goes into about.html, services.html, and appointment.html
Test: navigate between pages → dark mode stays on

Step 6 — Smooth transition effect
- Add a CSS transition on body so the color swap animates instead of snapping
Also swap the button icon (☀️ ↔ 🌙) to reflect the current mode
Test: toggle feels polished and icon updates correctly

Step 7 — Final visual review
- Scan each page for any hardcoded colors that bypass the CSS variables
Fix any contrast or visibility issues found
Each step is isolated, independently testable, and builds on the previous one. Ready to start with Step 1 whenever you are.
