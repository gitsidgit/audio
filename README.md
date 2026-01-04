# Dual Channel Audio Player

A compact, utilitarian dual-channel audio player built with Wavesurfer.js. This application allows you to load, play, and analyze two audio channels simultaneously with independent controls for each channel.

## Features

### Core Functionality
- **Dual Channel Support**: Load and play two independent audio tracks (Channel A and Channel B)
- **Synchronized Playback**: Both channels play in perfect sync with shared timeline
- **Waveform Visualization**: Each channel has its own waveform display with dual-timeline (top/bottom time markers)

### Channel Controls
- **Individual Channel Selection**: Click "A" or "B" to select which channel to load audio to
- **Independent Mute Controls**: Mute/unmute each channel separately
- **Channel Indicators**: Blue for Channel A, Red for Channel B
- **Active Channel Highlighting**: Visual indicator shows which channel is currently selected

### Playback Controls
- **Play/Pause**: Standard playback control (plays both channels)
- **Stop Button**: Stops playback and resets to beginning
- **Configurable Skip**: Forward/backward navigation with user-adjustable skip duration (0.1-60 seconds)
- **Loop Regions**: Drag on any waveform or minimap to create loop regions that automatically repeat

### Audio Controls
- **Volume Slider**: Adjust master volume
- **Global Mute**: Mute all channels simultaneously
- **Playback Speed**: Adjustable speed from 0.5x to 2.0x
- **Zoom Control**: Adjust waveform zoom level (10-500px per second)

### Visual Features
- **Dual Timeline**: Each waveform has top (blue) and bottom (purple) timelines for precise time navigation
- **Stacked Minimaps**: Separate minimap for each channel below main waveforms
- **Compact UI**: Tightly spaced controls for efficient use of space
- **Time Display**: Current time and total duration in header

## Usage

### Basic Operation
1. **Load Audio**: Click "Load Audio" button, select channel (A/B), then choose an audio file
2. **Play/Pause**: Click the play button or press Spacebar
3. **Navigate**: Use arrow buttons to skip forward/backward (default 5 seconds)
4. **Adjust Skip**: Change the number in the skip seconds input box to adjust navigation precision

### Channel Management
1. **Select Channel**: Click "A" or "B" button to select which channel to operate on
2. **Load Different Files**: Each channel can have its own audio file
3. **Independent Mute**: Use mute buttons to silence individual channels
4. **Channel Status**: Status indicator shows which channel is muted/unmuted

### Loop Regions
1. **Create Loop**: Drag on any waveform or minimap to create a loop region
2. **Play Loop**: Click on the colored region to play from that point
3. **Loop Behavior**: Playback automatically repeats within the region
4. **Remove Loop**: Click anywhere outside the region to remove it

### Keyboard Shortcuts
- **Space**: Play/Pause
- **Arrow Left/Right**: Skip backward/forward
- **S**: Stop playback
- **1/2**: Select Channel A/B
- **Ctrl+M**: Toggle global mute
- **ESC**: Remove all loop regions

## Technical Details

### Architecture
- **Framework**: jQuery + Wavesurfer.js v7.11.1
- **Plugins**: Minimap, Timeline, Regions
- **Container**: Single HTML file with embedded CSS and JavaScript
- **Audio Format**: Supports any browser-supported audio format (MP3, WAV, OGG, etc.)

### File Structure
- Single HTML file containing all code
- External dependencies loaded from CDN
- No build process required
- Works offline after initial load

### Browser Support
- Modern browsers with Web Audio API support
- Tested in Chrome, Firefox, Safari, and Edge
- Requires JavaScript enabled

## Setup

### Quick Start
1. Save the HTML file to your computer
2. Open it in any modern web browser
3. Start loading and playing audio files

### Hosting
- Can be hosted on any static web server
- No server-side processing required
- Works with local file system (file:// protocol)

## Use Cases

### Audio Analysis
- Compare two audio recordings side-by-side
- Analyze stereo channels independently
- Study timing relationships between channels

### Language Learning
- Load conversation recordings in separate channels
- Loop specific phrases or dialogue sections
- Adjust playback speed for comprehension

### Music Production
- Compare different mixes or takes
- Analyze stereo separation
- Study timing and synchronization

### Podcast Editing
- Separate host and guest audio tracks
- Create precise edit points with loop regions
- Adjust playback speed for transcription

## Limitations

- **File Size**: Large audio files may load slowly
- **Browser Memory**: Very long audio files may exceed browser memory limits
- **No Multi-track**: Limited to two channels (though each can be stereo)
- **Export**: No export functionality for edited regions
- **Undo**: No undo/redo functionality for region edits

## Credits

- Built with [Wavesurfer.js](https://wavesurfer-js.org/)
- jQuery for DOM manipulation
- Sample audio from [Audio Sample files](https://github.com/rafaelreis-hotmart/Audio-Sample-files)

## License

This project is provided as-is for educational and demonstration purposes. Feel free to modify and adapt for your needs.

## Contributing

Since this is a single-file demonstration, contributions would involve:
1. Forking the repository
2. Making improvements
3. Submitting a pull request

Or simply copy the code and adapt it for your specific use case.

---

*Note: This application stores audio files in browser memory. Large files may affect browser performance. All audio processing happens client-side; no data is sent to external servers.*