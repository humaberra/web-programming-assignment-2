# Web Programming - Assignment 2

## File Organization
- `index.html`: The core HTML file containing the document structure with 6 box elements (A through F). It dynamically connects to either `styleA.css` or `styleB.css`.
- `styleA.css`: Stylesheet implementing Version A. It uses Flexbox to align boxes vertically in the center, distributes spacing dynamically, alternates background colors, and centers the content of the final box.
- `styleB.css`: Stylesheet implementing Version B. It aligns boxes horizontally at the top-left using `inline-block` with `white-space: nowrap` to prevent wrapping, fixes the final box to the bottom-right corner, and handles hover transitions.
- `README.md`: Explains the repository structure and challenges encountered during implementation.

## Challenges Faced
1. **Dynamic Spacing without Shrinking (Style A):** Ensuring the vertical gap between boxes dynamically resized with the browser window while keeping the box dimensions strictly 100x100px. This was resolved using `justify-content: space-between` along with `flex-shrink: 0`.
2. **Preventing Line Wrapping (Style B):** Keeping the first five boxes on a single horizontal line even when resizing the window. Solved by setting `white-space: nowrap` on the parent container.
3. **Decoupling the Final Box (Style B):** Removing the last box (F) from the normal inline document flow and anchoring it strictly to the bottom-right corner using `position: fixed`.