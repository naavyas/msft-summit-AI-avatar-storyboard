# bnf-msft-avatar-dashboard
## Features

1. **Dynamic Video and Image Loading**
   - Uses the **File System Access API** to allow users to select a local directory of video or image files.
   - Displays the selected assets as tiles in the storyboard.

2. **Responsive Grid Layout**
   - Arranges tiles dynamically in a grid layout, adapting to the screen size and ensuring consistent spacing and alignment.

3. **Randomized Tile Behavior**
   - Introduces slight randomness to tile positioning and rotation, creating an organic and less rigid appearance.
   - Supports a custom range for tilting and positional offsets to prevent overlap.

4. **Interactive Enlarged View**
   - Users can click on any tile to enlarge it, bringing the corresponding video or image into focus.
   - Enlarged tiles play their video in full, with muted audio disabled, while background audio pauses for a seamless experience.

5. **Background Audio**
   - Plays a looping background audio file to enhance the immersive experience.
   - Background audio pauses automatically when a tile is enlarged and resumes when the enlarged view is exited.

6. **Performance Optimizations**
   - GPU-accelerated rendering via `transform` and `translateZ(0)` to ensure smooth transitions and responsiveness.
   - Clips video content using `border-radius` and `clip-path` to align with the rounded edges of the tiles.

7. **Fallbacks and Error Handling**
   - Handles missing or incompatible video files gracefully by providing console error messages and optional visual placeholders.
   - Includes a fallback for browsers that do not support the **File System Access API**.

---

## Technologies Used

- **HTML5**: Structure of the application and integration of multimedia content.
- **CSS3**: Styling of tiles, animations, transitions, and responsive layouts.
- **JavaScript (ES6)**: Dynamic behavior, file handling, and interactive features.
- **File System Access API**: Enables directory selection for custom video assets.
