WebRTC Video Chat
A real-time video chat application built with WebRTC, Firebase Firestore, and JavaScript. Connect with others instantly from anywhere using the live demo link below. The app supports multi-user video calls, audio/video toggling with dynamic icons, text chat, and a modern, responsive UI.
Live Demo
Access the app instantly: https://webrtc-70728.web.app
Note: Grant camera and microphone permissions in your browser to enable video and audio features.
Features

Video and Audio Streaming: Join multi-user video calls with peer-to-peer WebRTC connections.
Text Chat: Send and receive messages in real-time during calls.
Dynamic Controls:
Mute/unmute audio with mic icons (🎤 for unmuted, 🎙️ for muted).
Enable/disable video with camera icons (📷 for enabled, 📸 for disabled).
Green "Call" and "Answer" buttons to join, red "Hang Up" button to leave.

Peer Management: Automatically removes a user's video profile when they leave.
Responsive Design: Modern, mobile-friendly UI with hover effects and dark mode support.

Tech Stack

Frontend: HTML, CSS, JavaScript
WebRTC: For peer-to-peer video and audio streaming
Firebase Firestore: For signaling and peer coordination
Fonts: Inter and Syne Mono (via Google Fonts)

Usage

Open the App:

Visit "https://webrtc-70728.web.app" in a modern browser (Chrome, Firefox, Edge).
Allow camera and microphone access when prompted.

Join a Call:

Enter your username in the input field.
Click the green "Call" button to create a new room (generates a Room ID) or enter a Room ID and click the green "Answer" button to join an existing room.
Your webcam feed will start, and other participants' videos will appear.

Control Audio/Video:

Click "🎤 Mute Audio" to mute (changes to "🎙️ Unmute Audio").
Click "📷 Disable Video" to stop video (changes to "📸 Enable Video").

Chat:

Type a message in the chat input and click "Send" to communicate with others in the room.

Leave the Call:

Click the red "Hang Up" button to exit. Your video profile will be removed from other participants' screens.

Developer Instructions
For those interested in modifying or contributing to the project:

Clone the Repository
git clone https://github.com/AshanOdi/WebRTC-deployed.git
cd webrtc-video-chat

Install DependenciesInstall Firebase SDK:
npm install firebase

Configure Firebase

Create a Firebase project at Firebase Console.
Enable Firestore and copy your project credentials into main.js:const firebaseConfig = {
apiKey: "your-api-key",
authDomain: "your-auth-domain",
projectId: "your-project-id",
storageBucket: "your-storage-bucket",
messagingSenderId: "your-messaging-sender-id",
appId: "your-app-id",
measurementId: "your-measurement-id"
};

Run Locally for Testing

Start a local server:npm install -g live-server
live-server

Open http://localhost:8080 in your browser.

Project Structure
webrtc-video-chat/
├── index.html # Main HTML file
├── main.js # WebRTC and Firebase logic
├── style.css # UI styles
├── README.md # Project documentation
├── package.json # Node.js dependencies
└── .gitignore # Excludes node_modules, config files

![image](https://github.com/user-attachments/assets/a9d52d37-d639-410c-971e-601a65e8f5ea)

WebRTC for peer-to-peer communication
Firebase Firestore for signaling
Google Fonts for Inter and Syne Mono

Contact
For questions or feedback, open a GitHub issue or contact your-email@example.com.

Built with ❤️ using WebRTC and Firebase
