📌 **Project Title:** **Scenify - Image Scene Flow Organizer**  
📅 **Project Timeline:** **November 2026 – Present [Active Development & Maintenance]**  
🎥 YouTube Demo: TBD  
📦 GitHub Source Code: <https://github.com/Smart-Code-ACADEMY/2025.11.24_RND_software_workflow--Scenify>  

---

📍 My Personal Profiles ⬇︎  
🎥 Video Portfolio: To be added  
📦 GitHub Profile: <https://github.com/IvanSicaja>  
👔 LinkedIn: <https://www.linkedin.com/in/ivan-si%C4%8Daja-832682222>  
🎥 YouTube: <https://www.youtube.com/@ivan_sicaja>  

---

### 💡 Core Challenge This Project Resolves:

Designing and engineering a desktop image workflow system for visually organizing large image sequences into structured scene flows through thumbnail-based reordering, scene tagging, metadata-based favorites, controlled file renaming, preview navigation, search, and filesystem synchronization.

---

### 🔧 Core Skills Tree Used To Build The Project - Skills and Tech Stack:
*(Project-Specific Structured Overview)*
```
│
├── Software Engineering
│ ├── Software / Frameworks / Libraries
│ │ ├── Python
│ │ ├── PyQt5
│ │ ├── QSettings
│ │ ├── Qt Widgets
│ │ ├── Python os
│ │ ├── Python re
│ │ ├── Python struct
│ │ ├── Python zlib
│ │ └── piexif
│ │
│ └── Skills
│   ├── Desktop GUI application development
│   ├── Object-oriented software design
│   ├── Event-driven application architecture
│   ├── Thumbnail-based image navigation
│   ├── Drag-and-drop list reordering
│   ├── Keyboard-driven workflow design
│   ├── Persistent application settings
│   ├── Image preview & fullscreen visualization
│   └── File-system workflow automation
│
├── System Integration Engineering
│ ├── Software / Frameworks / Libraries
│ │ ├── PyQt5
│ │ ├── QSettings
│ │ ├── Windows Shell Integration
│ │ ├── EXIF Metadata
│ │ └── XMP Metadata
│ │
│ └── Skills
│   ├── GUI-to-filesystem integration
│   ├── Image metadata integration
│   ├── Windows Explorer rating integration
│   ├── Persistent metadata synchronization
│   ├── Folder-content monitoring
│   ├── Application-state persistence
│   ├── Thumbnail cache management
│   └── End-to-end image workflow integration
│
├── Image & Metadata Processing
│ ├── Software / Frameworks / Libraries
│ │ ├── PyQt5 QPixmap / QIcon
│ │ ├── EXIF
│ │ ├── XMP
│ │ ├── PNG iTXt
│ │ ├── piexif
│ │ └── Python binary file processing
│ │
│ └── Skills
│   ├── Image thumbnail generation & caching
│   ├── JPEG EXIF rating management
│   ├── JPEG / PNG XMP metadata management
│   ├── Scene-tag metadata embedding
│   ├── Persistent favorite ratings
│   ├── Image format validation
│   ├── Metadata-preserving workflow design
│   └── Windows Shell metadata refresh
│
└── Research & Development Engineering
  ├── Software / Frameworks / Libraries
  │ └── Integrated within sections above
  │
  └── Skills
    ├── Image workflow architecture
    ├── Scene-organization workflow design
    ├── Metadata interoperability research
    ├── File-renaming strategy development
    ├── User workflow optimization
    ├── Iterative GUI refinement
    └── Technical debugging & reliability improvement
```

<!-- Technical source: -->

---

### 📋 Core System Capabilities - List Only:

- **Image folder loading & thumbnail visualization**
- **Natural filename sorting**
- **Interactive image reordering**
- **Move selected images to top or bottom**
- **Scene-tag-based image grouping**
- **Move images to top or end of scene tags**
- **Persistent scene-tag metadata**
- **Persistent 5-star favorite ratings**
- **Favorites-only filtering**
- **Favorites export to dedicated folder**
- **Image preview with lock / unlock control**
- **Fullscreen image viewer**
- **Keyboard arrow navigation**
- **Image filename search**
- **Configurable thumbnail resizing**
- **Batch image renaming**
- **Selected-image renaming with configurable numbering**
- **Automatic detection of added / removed images**
- **Persistent window geometry & application state**
- **JPEG / PNG EXIF and XMP metadata integration**...

---

### 🧠️ How It Works - Core System Capabilities Workflow:

The project combines different software-engineering areas (**desktop GUI development, image organization, file-system automation, metadata processing, image previewing, structured renaming, scene grouping, persistent configuration, user workflow optimization...**)  
The core of the application is **Python**, **PyQt5**, **EXIF / XMP metadata processing**, and **filesystem-based image management**.

The application is also equipped with:

- **Thumbnail-based image organizer**
- **Scene-tag workflow**
- **Favorite rating system**
- **Fullscreen image viewer**
- **Batch file renaming**
- **Folder synchronization**
- **Persistent application settings**...

**Image folder loading:**  
Scenify loads supported image files including **JPG, JPEG, PNG, BMP, GIF, TIFF, TIF, and WEBP** from a selected folder. Files are naturally sorted and displayed as dynamically generated thumbnails with configurable thumbnail dimensions. A loading progress bar provides visual feedback while larger folders are being processed.

**Image scene flow organization:**  
Images can be reordered directly inside the thumbnail list through **drag-and-drop operations** or moved explicitly to the **top or bottom** of the sequence. Selection state and metadata overlays are rebuilt after list operations so the visual scene order remains synchronized with the application's internal representation.

**Scene tagging:**  
JPEG and PNG images can store persistent **scene tags** directly inside image metadata. Scenify uses EXIF / XMP metadata for JPEG files and XMP data inside PNG iTXt chunks. Scene tags are displayed within the interface and can be used to organize contiguous image groups representing individual scenes or sections.

**Scene-based navigation:**  
The application identifies scene-tag groups within the current image sequence. Selected images can be moved directly to the **top or end of a chosen scene-tag group**, and a scene-tag navigation control allows the user to jump directly between tagged sections.

**Favorite rating management:**  
JPEG, JPG, and PNG images support persistent favorite status through a **5-star metadata rating**. JPEG ratings are stored using EXIF and XMP metadata while PNG ratings are stored through XMP inside PNG metadata. Favorite states are read back when images are loaded, allowing the rating to persist between application sessions.

**Windows Explorer integration:**  
For supported JPEG images, Scenify writes rating information compatible with the Windows property system and triggers a Windows Shell change notification after metadata updates so Windows Explorer can refresh the corresponding file metadata.

**Image renaming:**  
Scenify supports both complete sequence renaming and selective renaming. Selected images can receive a configurable base name together with an adjustable zero-padded numeric suffix, while collision checks prevent duplicate filenames. Renamed images are repositioned according to natural filename sorting.

**Folder synchronization:**  
The application tracks the known contents of the active folder and detects files that have been added or removed. Newly discovered files can be incorporated through the reload workflow, while removed files are reflected in the interface so the image list remains synchronized with the actual filesystem.

**Image preview & navigation:**  
Selecting an image updates the integrated preview. The preview can be locked to a specific image, while keyboard navigation allows movement through the sequence with live preview updates. A dedicated fullscreen viewer provides an additional image-review workflow.

**Search & favorites:**  
Scenify provides filename-based search navigation and a **Favorites Only** workflow for focusing on rated images. Favorite images can also be copied into a dedicated `00_favorites` directory while keeping the original files unchanged.

**Persistent application state:**  
Qt **QSettings** stores window geometry, window state, and the last opened folder, allowing the working environment to be restored across application sessions.

---

### ⚠️ Note:

Persistent **ratings and scene-tag metadata** are implemented for **JPEG / JPG and PNG** files. Other supported image formats can be loaded and organized in Scenify but do not use the same embedded EXIF / XMP rating and scene-tag workflow.

---

### 📸 Project Snapshots:

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

<p align="center">
TBD
</p>

---

### 🎥 Video Demonstration:

<p align="center">
TBD
</p>

---

### 📣 Hashtags Section:

**#Scenify #ImageOrganizer #ImageWorkflow #SceneManagement #Python #PyQt5 #DesktopApplication #SystemIntegration #SoftwareEngineering #ImageMetadata #EXIF #XMP #FileSystemAutomation #WorkflowAutomation #ImageManagement #MetadataManagement #WindowsIntegration #GUI #ResearchAndDevelopment**