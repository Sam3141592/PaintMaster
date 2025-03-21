## PaintMaster  
**Course:** CIE 202 – Fundamentals of Computer Programming  
**Language:** C++

### Description
PaintMaster is an educational drawing application developed for kids, allowing them to create, modify, and play with shapes. The application features two modes: **Draw Mode** and **Play Mode**. It uses object-oriented programming principles and is built on top of a custom graphics library (CMU Graphics Library).

This project was part of the CIE 202 course at Zewail City and focuses on applying OOP design patterns, class hierarchies, and polymorphism to manage UI, drawing, and user interaction through a well-organized architecture.

---

### Features

#### Draw Mode
- Add figures: Rectangle, Triangle, Line, and Circle
- Select figures (highlight with information display)
- Change figure properties (color, fill, border width)
- Delete, Copy, Cut, Paste figures
- Save and Load graphs
- Switch between draw and play mode
- Exit with confirmation and optional saving

#### Play Mode
- Game mode using existing figures: Pick by shape, color, or both
- Score tracking based on correct and incorrect selections
- Restore original graph after gameplay
- Switch back to draw mode at any time

---

### Structure

#### Key Directories & Files
- `Actions/` – Contains all action classes (e.g., `AddRectAction`, `AddDeleteAction`, `ActionSave`)
- `Figures/` – Definitions for all figure types (e.g., `CRectangle`, `CCircle`, `CTriangle`)
- `GUI/` – Handles user interface and interaction (`Input`, `Output`, `UI_Info`)
- `CMUgraphicsLib/` – Integrated graphics library used for rendering and I/O
- `ApplicationManager.*` – Central class coordinating the app’s operations
- `main.cpp` – Entry point of the application
- `images/MenuItems/` – Toolbar icons used in the GUI

---

### How to Run
1. Open the solution file `PT-Project.sln` using **Visual Studio**.
2. Build the solution (make sure all required images and libraries are included).
3. Run the application.
4. Interact using the toolbar icons and drawing area.

---

### Object-Oriented Design Highlights
- Each figure type inherits from a common base class `CFigure`.
- Each operation (action) inherits from the base class `Action`.
- Full separation of concerns between GUI, application logic, and figures.
- Extensibility: Easily add new shapes or actions by extending the appropriate base class.
