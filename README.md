# AI Virtual Mouse 🖱️🤖  

An **AI-powered virtual mouse** that tracks hand gestures using **MediaPipe** and **OpenCV** to control your computer cursor and perform clicks.  

![Demo](demo.gif) *(Replace with an actual demo GIF later)*  

## Features ✨  
- **Hand Tracking**: Detects hand landmarks in real-time using **MediaPipe Hands**.  
- **Gesture Recognition**:  
  - 👆 **Cursor Movement**: Move your index finger to control the mouse.  
  - 🤏 **Click Gesture**: Pinch thumb and index finger to perform a left-click.  
  - ✌️ **Right-Click**: Use a different gesture (e.g., middle finger down) for right-click.  
- **Smooth Cursor Control**: Uses **PyAutoGUI** for seamless mouse movements.  
- **FPS Counter**: Displays real-time performance metrics.  

## Installation 🛠️  

### Prerequisites  
- Python 3.8+  
- OpenCV (`cv2`)  
- MediaPipe  
- PyAutoGUI  
- NumPy  

### Steps  
1. **Clone the repository**:  
   git clone https://github.com/yourusername/AI-virtual-mouse.git
   cd AI-virtual-mouse

2. **Set up a virtual environment (recommended)**:  
   python -m venv venv
   venv\Scripts\activate
   *(Alternatively, install manually: `pip install opencv-python mediapipe pyautogui numpy`)*  


## Customization ⚙️  
- **Adjust sensitivity**: Modify `smoothing_factor` in `config.py`.  
- **Change gestures**: Update `fingersUp()` logic in `handDetector.py`.  
- **Add new actions**: Extend `main.py` with PyAutoGUI functions (e.g., scrolling, dragging).  

## Troubleshooting 🛑  
|             Issue           |                           Solution                              |  
|-----------------------------|-----------------------------------------------------------------|  
| Camera not detected         | Try changing `cv2.VideoCapture(0)` to `(1)`                     |  
| Laggy cursor                | Reduce camera resolution in `main.py`                           |  
| PyAutoGUI permissions error | Grant accessibility permissions (Mac) or run as admin (Windows) |  

## Future Improvements 🔮  
- [ ] **Multi-hand support** (e.g., two-handed gestures).  
- [ ] **Voice commands** integration.  
- [ ] **Custom gesture training** (ML model).  
