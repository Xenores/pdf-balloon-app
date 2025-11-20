
# PDF/Image Annotation Tool (Balloon & Leader-Line Editor)

*A web app for creating annotations on CAD drawings (PDF or image files)*

**Live demo:** [https://xenores.github.io/pdf-balloon-app/](https://xenores.github.io/pdf-balloon-app/)

---

## Overview

This tool enables users to open a PDF or image file (e.g., CAD drawings, architectural/engineering PDFs), and add **balloons**, **leader lines**, and **text-boxes** as annotations. It supports zooming, dragging annotations, saving/loading projects, and exporting a final annotated PDF.

Built as a solution to simplify annotation workflows during my internship, the app runs entirely in the browser (no backend required).

---

## Features

* Open PDFs or images (.png, .jpg, .jpeg, .webp)
* Add numbered annotation balloons
* Drag & reposition balloons (grid snapping supported)
* Change balloon color, size, font
* Create leader lines attached to balloons
* Draggable line endpoints
* Add editable text boxes
* Working zoom with proper annotation scaling
* Undo support
* Save project as JSON
* Load saved projects
* Export annotated PDF
* Pure client-side app (no upload to servers)

---

## How to Use

### 1. Load a File

Click **“Select File”** and choose a PDF or image.

### 2. Add Balloons

* Hold **Ctrl + Click** anywhere to place a balloon
* Drag to move it
* Right-click → delete
* Double-click → rename

### 3. Leader Lines

* Enable **Line Mode**
* After pacing a balloon, hold **Ctrl + Click** to create a line
* Move endpoints using handles

### 4. Text Box Mode

* Enable **Text Field Mode**
* Click to create text box
* Edit directly, drag to move, press **Delete** to remove

### 5. Save / Load Projects

* **Save Project** → downloads a JSON file containing annotations
* **Open Project** → load saved annotations + original PDF/image

### 6. Export

Export to a PDF with annotations rendered at the current zoom level.

---

## Author

**Aravind Kavanal Sreeni**
Built as part of an internship initiative to simplify CAD drawing annotation workflows.

GitHub: [https://github.com/Xenores](https://github.com/Xenores)
LinkedIn: [https://linkedin.com/in/aravind-k-s](https://linkedin.com/in/aravind-k-s)

---

