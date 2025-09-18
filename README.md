# Marker Based AR

A Unity-based augmented reality application that uses marker detection to overlay digital content in the real world. This project utilizes Vuforia AR platform for robust marker tracking and AR functionality.

## Project Overview

This application demonstrates marker-based augmented reality technology where virtual objects and animations are rendered when specific markers are detected by the device camera. The project includes dance animation content that is triggered when markers are recognized.

## Features

- Marker-based AR tracking using Vuforia
- 3D character animations (Wave Hip Hop Dance)
- Real-time camera feed processing
- Cross-platform compatibility (iOS/Android)

## Requirements

### Software Requirements
- Unity 2019.4 LTS or later
- Vuforia Engine 11.1.3
- Android SDK (for Android builds)
- Xcode (for iOS builds)

### Hardware Requirements
- Device with camera support
- Minimum Android 7.0 (API level 24) or iOS 12.0
- ARCore/ARKit compatible device recommended

## Setup Instructions

1. **Clone the Repository**
   ```
   git clone <repository-url>
   cd "Marker Based AR"
   ```

2. **Open in Unity**
   - Launch Unity Hub
   - Click "Open Project"
   - Navigate to the cloned repository folder
   - Select the project folder

3. **Vuforia Configuration**
   - The project already includes Vuforia Engine 11.1.3
   - Vuforia configuration is located in `Assets/Resources/VuforiaConfiguration.asset`
   - You may need to update the license key in the Vuforia Configuration

4. **Build Settings**
   - Go to File > Build Settings
   - Select your target platform (Android/iOS)
   - Configure platform-specific settings as needed

## Project Structure

```
Assets/
├── Editor/              # Editor-only scripts and tools
├── Player/              # Runtime player assets
│   ├── Wave Hip Hop Dance 1.controller  # Animation controller
│   └── Wave Hip Hop Dance.fbx           # 3D dance animation
├── Resources/           # Runtime resources
│   └── VuforiaConfiguration.asset       # Vuforia settings
├── Scenes/             # Unity scenes
└── StreamingAssets/    # Platform-specific streaming assets
```

## Usage

1. **Testing in Unity Editor**
   - Open the main scene from `Assets/Scenes/`
   - Press Play to start the AR session
   - Point the camera at configured markers

2. **Building for Mobile**
   - Configure build settings for your target platform
   - Build and deploy to your device
   - Grant camera permissions when prompted
   - Point device camera at markers to see AR content

## Markers

This application uses predefined image markers for tracking. Ensure you have the correct marker images that correspond to the Vuforia database configuration.

## Development Notes

- The project uses Unity's legacy input system
- Vuforia handles the AR camera and tracking
- Animation system uses Unity's Animator Controller
- Built APK is included in the root directory for testing purposes

## Troubleshooting

### Common Issues
- **Camera not working**: Ensure camera permissions are granted
- **Markers not detected**: Check lighting conditions and marker quality
- **Build errors**: Verify Unity version compatibility and platform SDKs

### Performance Optimization
- Test on target devices regularly
- Monitor frame rate and memory usage
- Optimize texture sizes and polygon counts for mobile devices

## License

This project is for educational and demonstration purposes. Please ensure compliance with Vuforia's license terms for commercial use.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly on target devices
5. Submit a pull request

## Contact

For questions or support regarding this AR application, please open an issue in the repository.