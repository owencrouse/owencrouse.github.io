# 3D Interactive Classroom Portfolio

An immersive 3D virtual classroom built with Three.js that serves as an interactive portfolio and resume showcase. Explore the classroom environment to discover professional information, projects, and contact details in a unique and engaging way.

## Project Overview

This project transforms a traditional portfolio website into an interactive 3D experience. Users can navigate through a detailed classroom environment, interact with various objects, and access professional information through clickable elements.

## Key Features

### Interactive Elements
- **Teacher's Computer** - Click the monitor screen to open a Windows XP-styled interface with links to:
  - Resume/CV
  - GitHub profile
  - LinkedIn profile
  - Email contact
  - Additional portfolio pages

- **Filing Cabinet** - Three interactive drawers containing:
  - **Top Drawer**: Featured projects and technical implementations
  - **Middle Drawer**: Education history and technical skills
  - **Bottom Drawer**: Work experience and professional background

- **Blackboard** - Click to zoom to the back of the classroom for a different perspective view

### Visual Features
- Real-time working clock with accurate hour, minute, and second hands
- Animated ceiling fan
- Pulsing window lighting effects
- Subtle desk and chair animations
- Custom poster displays on walls
- student desks with computers
- Teacher's desk with retro CRT computer setup

## Technologies Used

- **Three.js (r128)** - 3D graphics rendering
- **JavaScript (ES6)** - Core functionality and interactions
- **HTML5/CSS3** - Structure and styling
- **Raycasting** - Click detection and object interaction
- **Canvas API** - Dynamic texture generation for blackboard text

## Technical Highlights

### 3D Scene Architecture
- Modular object creation (desks, chairs, computers, filing cabinet)
- Proper shadow mapping and lighting setup
- Fog effects for depth perception
- Responsive camera animations with smooth transitions

### Interaction System
- Raycaster-based click detection
- Recursive object hierarchy traversal
- State management for drawer open/close states
- Overlay UI system with Windows XP theming

### Performance Optimizations
- Efficient geometry reuse
- Optimized shadow map resolution (2048x2048)
- PCF soft shadows for realistic lighting
- Minimal draw calls through grouped objects

## Project Structure
```
├── index.html              # Main classroom scene
├── images/                 # Texture images for posters and UI
│   ├── resume_img.png
│   ├── inception_testposter.jpg
│   ├── tron-motorcycle.jpg
│   ├── github_img.webp
│   ├── linkedin_img.png
│   └── gmail_img.png
├── icons/                  # Icons for computer interface
│   ├── tech-icon.png
│   └── simulator-icon.png
└── loadingscreen.html      # External linked pages
```

## How It Works

1. **Scene Initialization**: Creates the 3D environment with classroom elements
2. **Event Listeners**: Monitors mouse clicks and window resizing
3. **Raycasting**: Detects which 3D objects are clicked
4. **Camera Animation**: Smoothly transitions between views (default, computer zoom, blackboard)
5. **Dynamic UI**: Generates HTML overlays for computer and filing cabinet content
6. **Animation Loop**: Continuously updates clock, fan rotation, and ambient animations

## Learning Outcomes

This project demonstrates proficiency in:
- 3D graphics programming and spatial reasoning
- Event-driven architecture and user interaction design
- State management in complex applications
- Creative problem-solving for portfolio presentation
- Integration of multiple web technologies

## Design Philosophy

The classroom metaphor represents a learning environment where visitors can "attend class" and discover information about Owen Crouse's professional journey. Each interactive element reveals different aspects of my qualifications, creating an 
engaging narrative experience rather than a static document. I also plan on adding educational topics which will allow user to learn about various tech subjects through video links, animation, and notes provided. 

## Customization

To personalize this project:
1. Replace image files in `/images` and `/icons` directories
2. Update links in `createComputerUI()` function
3. Modify drawer content in `showDrawerDocument()` function
4. Adjust blackboard text in the canvas texture generation
5. Add or remove classroom elements as desired

## License

This project is open source and available for educational purposes.

---

**Created by Owen Crouse** | [GitHub](https://github.com/owencrouse) | [LinkedIn](https://www.linkedin.com/in/owen-crouse-821989318)
