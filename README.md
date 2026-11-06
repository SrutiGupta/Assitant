# 🤖 AI-Powered Virtual Assistant

**A personalized AI-powered virtual assistant that understands voice commands, processes natural language, and performs intelligent actions using Google's Gemini API.**

AI-Powered Virtual Assistant is a full-stack web application built using the MERN stack that enables users to interact with their own customizable AI assistant through voice and text commands.

Powered by Google's Gemini API and the Web Speech API, the application understands user instructions, identifies their intent, and routes requests to appropriate actions such as Google Search, YouTube, Wikipedia, Google Maps, weather information, calculations, and date/time queries.

Users can personalize their assistant by choosing its name and avatar, creating a more interactive and personalized assistant experience.

## ✨ Key Features

- **🧠 AI-Powered Intent Recognition:** Uses Google Gemini API to understand natural language commands and determine the appropriate action.
- **🎙️ Voice Interaction:** Supports speech-to-text using the browser's Web Speech API.
- **🔊 Text-to-Speech:** Converts assistant responses into speech for a conversational experience.
- **🎨 Customizable Assistant:** Allows users to personalize their assistant with a custom name and avatar.
- **🔐 Secure Authentication:** Implements JWT-based authentication and password hashing using bcrypt.
- **☁️ Cloud Image Storage:** Uses Cloudinary for uploading and managing assistant profile images.
- **🔎 Google Search:** Routes search requests to Google Search.
- **▶️ YouTube Integration:** Supports YouTube-related voice and text commands.
- **📚 Wikipedia Integration:** Handles requests for information through Wikipedia.
- **📍 Google Maps Integration:** Supports location and navigation-related requests.
- **🌦️ Weather Information:** Handles weather-related queries.
- **🧮 Calculator:** Processes mathematical calculations.
- **📅 Date & Time:** Handles date and time-related queries.
- **💾 User Data Management:** Stores user profiles and relevant application history in MongoDB.
- **⚡ Intelligent Command Routing:** Uses Gemini-generated structured JSON responses to identify user intent and route commands to the corresponding functionality.

## 🧰 Tech Stack

| Category | Technologies |
|---|---|
| Frontend | React.js |
| Backend | Node.js, Express.js |
| Database | MongoDB |
| AI Integration | Google Gemini API |
| Authentication | JWT, bcrypt |
| Voice Recognition | Web Speech API |
| Speech Synthesis | Web Speech API |
| Image Storage | Cloudinary |
| File Uploads | Multer |
| Architecture | MERN Stack |
| API Communication | REST APIs |

## 🏗️ Application Workflow

The assistant follows an AI-powered command-processing workflow:

1. **User Input:** The user provides a voice or text command.
2. **Speech Recognition:** Voice input is converted into text using the Web Speech API.
3. **Intent Recognition:** The Gemini API processes the command and identifies the user's intent.
4. **Structured Response:** Gemini generates structured JSON describing the recognized intent and relevant information.
5. **Command Routing:** The application routes the recognized intent to the corresponding functionality.
6. **Action Execution:** The appropriate action is triggered, such as opening Google Search, YouTube, Maps, or processing a calculation.
7. **Assistant Response:** The assistant responds through text and, where supported, speech synthesis.

## 🚀 Getting Started

### Prerequisites

Before running the application, ensure you have:

- Node.js and npm installed.
- MongoDB database (local or cloud).
- Google Gemini API key.
- Cloudinary account and API credentials.

### 1. Clone the Repository

```bash
git clone https://github.com/SrutiGupta/AI-Virtual-Assistant.git
cd AI-Virtual-Assistant
```

### 2. Install Dependencies

Install frontend and backend dependencies separately.

**Backend**

```bash
cd backend
npm install
```

**Frontend**

```bash
cd ../frontend
npm install
```

### 3. Configure Environment Variables

Create a `.env` file inside the backend directory.

```env
PORT=8000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

Replace the example values with your actual credentials.

**Important:** Never commit your `.env` file, API keys, database credentials, or other sensitive information to GitHub.

### 4. Run the Application

Start the backend server:

```bash
cd backend
npm run dev
```

Start the frontend in a separate terminal:

```bash
cd frontend
npm run dev
```

Open the local URL displayed by your frontend development server in your browser.

*Note: The directory names, environment variable names, port, and npm scripts should match the actual repository configuration.*

## 🔐 Authentication & Personalization

The application provides user authentication and personalized assistant management.

- JWT-based authentication.
- Password hashing using bcrypt.
- HTTP-only cookie-based authentication.
- Individual user profiles.
- Custom assistant names.
- Custom assistant avatars.
- MongoDB-based profile and history storage.

## 🎯 Supported Assistant Actions

| Feature | Functionality |
|---|---|
| Google Search | Handles web search requests |
| YouTube | Routes YouTube-related commands |
| Wikipedia | Handles information lookup requests |
| Google Maps | Supports location-related commands |
| Weather | Handles weather queries |
| Calculator | Processes mathematical expressions |
| Date & Time | Handles time-related requests |

The Gemini API is responsible for interpreting user intent and generating structured routing information. The application handles the actual command execution.

## 🎙️ Voice Interaction

The application uses browser-native speech capabilities to create a voice-based interaction experience.

**Speech-to-Text**
- Captures voice input using the Web Speech API.
- Converts spoken commands into text.
- Checks commands against the personalized assistant name.

**Text-to-Speech**
- Uses browser speech synthesis to convert assistant responses into audio.
- Provides a more conversational user experience.

## ☁️ Cloud Image Management

Cloudinary is integrated for assistant avatar uploads.

The upload workflow uses:
- Multer for handling incoming file uploads.
- Cloudinary for cloud-based image storage.
- MongoDB for storing relevant user profile information.

## 🔒 Security

The application incorporates several security mechanisms:

- JWT-based authentication.
- HTTP-only cookies for authentication token handling.
- bcrypt password hashing.
- User-specific profile management.
- Environment-based configuration for sensitive credentials.

## 🤝 Contributing

Contributions and suggestions are welcome!

1. Fork the repository.
2. Create a new feature branch.
3. Implement your changes.
4. Test the functionality.
5. Submit a pull request with a clear description.

## 👩‍💻 Author

**Sruti Gupta**

AI-Powered Full Stack Developer

- GitHub: [@SrutiGupta](https://github.com/SrutiGupta)
- Project Repository: [AI-Powered Virtual Assistant](https://github.com/SrutiGupta/AI-Virtual-Assistant)

---

<p align="center">
  <b>Making everyday interactions smarter through AI, voice, and intelligent automation.</b>
</p>
