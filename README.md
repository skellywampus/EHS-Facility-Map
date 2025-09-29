<img src="https://github.com/skellywampus/EHS-Facility-Map/blob/main/Screenshot.png" alt="">

# Facility Map Viewer & Editor

This is a self-contained, browser-based facility map tool designed for environmental, health, and safety (EHS) applications. It allows organizations to visually manage and annotate site maps with key safety infrastructure such as:

- Fire Extinguishers  
- Spill Kits  
- Emergency Showers  
- Eyewashes  
- Emission Points  
- Stormwater Outfalls  
- Bulk Chemical Storage  
- Waste Accumulation Areas  
- Safer Areas  
- Evacuation Points  

## Features

- ✅ Toggleable layers for each item type  
- ✅ Admin login for placing, labeling, and saving pins  
- ✅ Pins are saved directly in the HTML file—fully self-contained  
- ✅ Optional printing support with only visible legend items included  
- ✅ Exportable image with visible markers  
- ✅ No server required, only a shared network drive.

---

## How to Use

### Setup

1. Place your site image in the same directory and name it:  
   `facility-map.png`  
   (Required format: PNG)

2. Open `index.html` in any modern browser.  
   No internet connection or installation required.

---

### User Mode

- Hover over pins to view item type and label (if applicable).  
- Use checkboxes in the legend to toggle visibility of layers.  
- Use zoom and rotate controls to adjust view.

---

### Admin Mode

1. Click "Admin Login" and enter password: `EHS-Admin` (case-sensitive)  
2. Select item type from the dropdown  
3. Click "Toggle Add Mode"  
4. Click on the map to drop pins  
5. If the item requires a label (e.g., Spill Kit, EP, etc.), a prompt will appear  
6. Click "Save Layout" to export a new version of the HTML file with pins embedded  
7. Optional: Click "Print" to generate a print-friendly map

> Admin mode visibility is not preserved when saving—the exported HTML will always load in user mode by default.

---

## Printing

- Use the **Print** button or your browser's print dialog.  
- Only layers currently visible will appear in the printout.  
- Legend is auto-positioned and filtered accordingly.  
- Recommended: "Fit to Page" and landscape orientation for best results.

---

## License

[MIT License]

---

## Notes

- This project does not require any backend, dependencies, or frameworks.  
- To share updates across a network, replace the original `index.html` with the newly exported `index.html`.

---

## Customization

- To change the admin password, locate this line in the HTML:

```
  const ADMIN_PWD = "EHS-Admin";
