<img src="https://github.com/skellywampus/EHS-Facility-Map/blob/main/Screenshot.png" alt="">

# Facility Map Viewer & Editor

A self-contained, browser-based facility map system for Environmental, Health, and Safety (EHS) management.  
It provides a visual, interactive method to locate, label, and document key safety assets within a facility.

---

## Key Capabilities

### General
- Fully self-contained — all data (pins, marker types, configuration) stored inside the HTML file.
- No server, database, or external dependencies required.
- Works directly from a shared network drive.
- Cross-browser compatible; tested in Chrome, Edge, and Orion.

### Map & Visualization
- Toggle visibility of individual item types via the dynamic legend.
- Zoom, rotate, and pan with mouse or controls.
- Tooltip display of item type and label on hover.
- Real-time pin placement, movement, and deletion (admin only).

### Admin Features
- Password-protected admin mode.
- Add, edit, or delete marker **types** (shape, color, labeled flag, abbreviation).
- Add, move, or delete **pins** for all marker types.
- Import pins from an existing HTML file.
- Export/save new layouts as a single updated HTML file.
- Change admin password within the interface (persists after saving layout).
- Manage all marker types and pins via popup modals.

### Persistence
- All edits (pins, marker types, password changes) are embedded directly into the exported HTML.
- The saved file becomes the new working copy—no additional configuration files required.

### Printing
- **Print Map:** Standard print view with visible markers.  
- **Print w/ Labels:** Generates labeled map with (mostly) non-overlapping tags and red leader lines.  
- Only currently visible legend items appear in the printout.
- Automatically adds emergency shower/eyewash note when applicable. (Assumes that showers are plumbed with built in eyewash)

---

## How to Use

### Setup
1. Place your site map image in the same folder and name it:
```facility-map.png```
*(PNG format required)*

2. Open `index.html` in any modern browser.  
*(No installation or internet required.)*

---

### User Mode
- Hover over pins to display type and label.
- Toggle layers via legend checkboxes.
- Adjust zoom and rotation as needed.
- Print or export without requiring admin access.

---

### Admin Mode
1. Enter the password (default: `EHS-Admin`).
- Note that this password is available to view as plaintext if the user opens the html in a text editor. This isn't true security, just enough to keep accidents from happening.
3. Access all management tools:
- Add new marker types or remove unused ones.
- Modify type properties (shape, color, labeled status, abbreviation).
- Toggle add mode and click map to drop new pins.
- Manage existing pins from the admin table modal.
- Import pins from prior versions.
- Change password and save layout to persist all updates.
3. Click **Save Layout** to download a new, fully updated version of the HTML file.

> The exported file always opens in user mode by default.

---

## Printing
- Use **Print** for a basic visible map or **Print w/ Labels** for annotated output.  
- Only visible layers are included.
- Shower note appears only when Emergency Showers are displayed. (Assumes that showers are plumbed with built in eyewash)
- Recommended settings: *Landscape orientation*, *Fit to Page*.

---

## License
[MIT License]

---

## Notes
- The system functions entirely client-side.
- Updates are distributed simply by replacing the shared `index.html` file.
- Ideal for compliance documentation, safety audits, and environmental reporting.
