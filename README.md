# PeerJS Conference

A real-time video conferencing web application built with PeerJS for peer-to-peer WebRTC connections.

## Features

- **Peer-to-Peer Video Calls**: Direct browser-to-browser video communication using WebRTC
- **Room-based Conferencing**: Join rooms using URL hashes (e.g., `#my-room`)
- **Camera Management**: 
  - Switch between multiple cameras
  - Camera availability detection and caching
  - Remember last used camera
- **Media Controls**:
  - Toggle video on/off
  - Toggle audio on/off
  - Visual indicators for muted states
- **Stream Monitoring**: Real-time monitoring of stream status with online/offline indicators
- **Participant Management**: 
  - Automatic participant discovery
  - Real-time participant count
  - Host-based room coordination
- **Responsive Design**: Adaptive video grid layout for various screen sizes

## How to Use

1. **Access the Application**: Open `index.html` in a web browser
2. **Join a Room**: 
   - Use the default room or specify a room in the URL hash: `#your-room-name`
   - The first participant in a room becomes the host
3. **Grant Permissions**: Allow camera and microphone access when prompted
4. **Start Conferencing**:
   - Participants automatically connect to each other
   - Video streams are displayed in a responsive grid
5. **Use Controls**:
   - Video toggle: Enable/disable camera
   - Audio toggle: Mute/unmute microphone
   - Camera switch: Cycle between available cameras

## Technical Details

### Architecture
- **Frontend**: Pure HTML, CSS, and JavaScript
- **Signaling**: PeerJS for WebRTC signaling and peer discovery
- **Media**: WebRTC for real-time audio/video communication
- **Storage**: LocalStorage for camera preferences and availability cache

### Key Components
- **Peer Management**: Automatic peer connection and call establishment
- **Stream Handling**: Real-time stream monitoring and quality detection
- **Error Handling**: Comprehensive error handling with automatic retries
- **Connection Recovery**: Automatic page reload on connection failures

### Browser Compatibility
- Modern browsers with WebRTC support
- HTTPS required for media device access
- Mobile browser compatible

## Setup

No build process or dependencies required. Simply:

1. Clone or download the repository
2. Open `index.html` in a web browser
3. The application will automatically load PeerJS from CDN

## Configuration

The application uses default PeerJS configuration:
```javascript
{
    host: '0.peerjs.com',
    port: 443,
    path: '/',
    debug: 3
}
```


# [Meet demo](https://fast-chat.github.io/meet/)

```
https://fast-chat.github.io/meet/
https://fast-chat.github.io/meet/#room-id
https://fast-chat.github.io/meet/#any-name-for-room-id
```


# Donate

ETH: 0x57E9A8FE46dBa5650898B3469E44391972263950
