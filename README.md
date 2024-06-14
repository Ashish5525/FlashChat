# FlashChat
Flash Chat is a real-time chat application designed for iOS devices. The app leverages Firebase for backend services, including authentication and data storage, to deliver a seamless and dynamic chatting experience.

## Features

### User Authentication
- **Email and Password Registration:** Users can create accounts using their email addresses and passwords.

### Real-Time Chat
- **Messaging:** Users can send and receive messages in real-time. Messages are stored in Firebase Firestore, allowing for instant updates and retrieval.
- **Auto-Scrolling Interface:** The chat interface auto-scrolls to the latest message, ensuring a smooth user experience.
- **User-Specific UI:** The app distinguishes between messages sent by the current user and those sent by others, customizing the UI accordingly.
### User Experience Enhancements
- **Animated Welcome Screen:** Features an engaging welcome animation using UILabel.
- **IQKeyboardManager Integration:** Ensures that the keyboard behaves seamlessly with the user interface, automatically handling text fields and dismissing the keyboard on outside touches.

### Requirements
- iOS 13.0+
- Xcode 12+
- CocoaPods for dependency management

# Installation

## 1. Clone the Repository
```bash
git clone https://github.com/yourusername/flash-chat-ios.git
cd flash-chat-ios
```

## 2. Install Dependencies
Install the required CocoaPods dependencies:
```bash
pod install
```

## 3. Configure Firebase

- Create a new project in the Firebase Console.
- Add an iOS app to your Firebase project.
- Download the GoogleService-Info.plist file and add it to your Xcode project.
  
## 4. Open the Project
Open the project workspace in Xcode:
```bash
open FlashChat.xcworkspace
```
# Usage
## Running the App
1. Build and run the app in Xcode.
2. Register a new user with an email and password, or use the phone number authentication feature to receive an OTP and log in.
Project Structure

## Main Components
- **AppDelegate.swift:** Configures Firebase and IQKeyboardManager during the app launch.
- **SceneDelegate.swift:** Manages the lifecycle of the app's scenes.
- **WelcomeViewController.swift**: Displays an animated welcome screen with a custom title animation.
- **RegisterViewController.swift**: Handles user registration via email/password and phone number OTP.
- **LoginViewController.swift:** Manages user login with email and password.
- **ChatViewController.swift:** Displays the chat interface, handles message sending and receiving, and updates the UI in real-time.
  
## Firebase Integration
- **Firebase Authentication:** Manages user sign-up and sign-in processes using email/password and phone number authentication.
- **Firestore:** Stores and retrieves chat messages in real-time, enabling a dynamic and interactive chat experience.
  
## User Interface
- **Storyboard:** Utilizes a storyboard for designing the UI components and setting up segues between different view controllers.
- **Custom Cells:** Implements custom table view cells to display chat messages with distinct styles for sent and received messages.

# License

This project is licensed under the Apache-2.0 License - see the LICENSE file for details.

