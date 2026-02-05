# University of Washington Web Map Tilesets (Mapbox GL JS)

## 🌐 Web Map URL
https://vipshehbaz.github.io/YOUR_REPOSITORY_NAME

> This interactive web map visualizes multiple raster tile sets generated in QGIS and rendered using Mapbox GL JS.

---

## 📍 Examined Geographic Area
**University of Washington (UW) Campus, Seattle, Washington, USA**

The study area focuses on the central UW campus near Husky Stadium, including selected campus buildings digitized manually in QGIS. The extent was intentionally limited to reduce tile count and comply with GitHub Pages file-size constraints.

---

## 🗺️ Tile Sets Description

### **Tileset #1 — Custom Basemap (Mapbox Studio)**
- **Source**: Mapbox Studio
- **Type**: Vector basemap (served via Mapbox style URL)
- **Design**:
  - Monochrome / muted color scheme
  - Reduced visual contrast
  - Modified land, water, and road colors
  - Customized label font and reduced POI clutter
- **Purpose**:
  - Provide geographic context
  - Serve as a neutral background for thematic layers
- **Zoom Levels**: Controlled by Mapbox (default basemap behavior)

📸 *Screenshot:*  
![Tileset 1](screenshots/tileset1_basemap.png)

---

### **Tileset #2 — Digitized UW Buildings (Thematic Layer)**
- **Source**: Manually digitized polygon layer in QGIS
- **Data Type**: Raster tiles exported from vector building polygons
- **Content**:
  - 9 campus building footprints
  - Attribute table includes building identifiers
  - Labels rendered at appropriate zoom levels
- **Purpose**:
  - Highlight selected campus buildings as a thematic layer
- **Zoom Levels**: 11–15

📸 *Screenshot:*  
![Tileset 2](screenshots/tileset2_buildings.png)

---

### **Tileset #3 — Buildings + Basemap (Composite Raster)**
- **Source**:
  - Tileset #2 (digitized buildings)
  - OpenStreetMap basemap rendered and muted in QGIS
- **Data Type**: Raster tiles
- **Purpose**:
  - Demonstrate exporting a composite map layer from QGIS
  - Preserve cartographic styling as a static raster tileset
- **Zoom Levels**: 11–15

📸 *Screenshot:*  
![Tileset 3](screenshots/tileset3_composite.png)

---

### **Tileset #4 — Thematic Mask Map**
- **Source**: QGIS
- **Design**:
  - Mask-based thematic visualization
  - Non-selected areas visually muted
  - Emphasis placed on selected campus features
- **Purpose**:
  - Demonstrate thematic cartographic design
  - Apply visual hierarchy and focus
- **Zoom Levels**: 11–15

📸 *Screenshot:*  
![Tileset 4](screenshots/tileset4_theme.png)

---

## 🧩 Web Map Features

- Fullscreen interactive map
- Custom Mapbox basemap (Tileset #1)
- Raster tile overlays (Tilesets #2, #3, #4)
- Layer switcher to toggle thematic layers
- Zoom and scale controls
- Map title and description overlay
- Hosted via **GitHub Pages**

---

## 🗂️ Repository Structure

[your_repository_name]/
├─ readme.md
├─ index.html
└─ assets/
├─ tileset_2/
│ └─ {z}/{x}/{y}.png
├─ tileset_3/
│ └─ {z}/{x}/{y}.png
└─ tileset_4/
└─ {z}/{x}/{y}.png


---

## 🛠️ Tools & Technologies Used

- **QGIS** — data digitization, cartographic styling, raster tile export
- **Mapbox Studio** — custom basemap design
- **Mapbox GL JS** — interactive web map rendering
- **GitHub Pages** — web hosting

---

## 📌 Notes

- Export extents and zoom ranges were intentionally limited to avoid excessive tile generation.
- Raster tiles follow the standard `{z}/{x}/{y}.png` web tile pyramid structure.
- All map layers were designed with visual hierarchy and cartographic clarity in mind.

---

## 👤 Author

Malaika

