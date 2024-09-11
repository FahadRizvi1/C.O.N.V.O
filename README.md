# Real-Time Video Chat Application(C.O.N.V.O)


This project is a real-time video chat application built using Agora's RTM (Real-Time Messaging) SDK and WebRTC. Users can create or join video chat rooms via a simple user interface.

Features
Create or Join Rooms: Users can join a video chat room by entering an invite code.
Real-Time Communication: Peer-to-peer video communication using WebRTC and STUN servers.
Camera & Microphone Control: Users can toggle their camera and microphone on or off during a call.
User Interface: Simple and intuitive user interface with a form to join rooms.


Project Structure
lobby.html: The entry point where users can join or create rooms by providing an invite link. It also handles redirection to the video chat room.
main.js: Manages the core functionality of the application, including setting up the video chat connection, handling new participants, sending/receiving video streams, and toggling the camera and microphone.


How It Works
Join/Create Room: The user submits a room code in the lobby page (lobby.html). If no code is provided, the app redirects back to the lobby.
Video Connection: Using WebRTC, the app captures audio and video, and establishes peer-to-peer connections through STUN servers.
Agora RTM: Agora is used to manage room membership and send signaling messages for WebRTC (offers, answers, and ICE candidates).


UI Elements:

#user-1: The local video stream.

#user-2: The remote participant’s video stream.
Buttons to toggle camera and microphone during the call.

Set up your Agora app by registering for an Agora account and getting an APP_ID.

Update the main.js file with your Agora APP_ID.
let APP_ID = "your-agora-app-id";

Open lobby.html in a browser to start the application.

Technologies Used
Agora SDK: Handles real-time messaging and room management.
WebRTC: Peer-to-peer video and audio streaming.
HTML/CSS/JavaScript: Frontend development.


Usage
Open the lobby.html in your browser.
Enter a room code and click "Join Room."
Allow access to your camera and microphone.
Toggle the camera or mic using the buttons provided.


Future Improvements
Add support for multiple participants.
Implement authentication for more secure room access.
Improve the user interface design.
