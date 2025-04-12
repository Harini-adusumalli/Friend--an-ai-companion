# Friend--an-ai-companion
# AI Friend - Mental Health Wellness Platform

AI Friend is a web-based mental health wellness platform that provides users with an AI companion for emotional support, mood tracking, and self-care guidance.

## Features

- 🤖 AI-powered chat companion for emotional support
- 📝 Journaling functionality
- 📊 Mood tracking and analysis
- 🧘 Self-care recommendations
- 🔒 Secure user authentication
- 💬 Real-time chat interface
- 📱 Responsive design for all devices

## Tech Stack

- Frontend: HTML, CSS, JavaScript
- Backend: Node.js, Express
- Database: MongoDB
- AI Integration: Google Gemini AI
- Authentication: JWT, bcrypt

## Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)
- MongoDB
- Google Gemini AI API key

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ai-friend.git
cd ai-friend
```

2. Install dependencies:
```bash
npm install
```

3. Environment Setup:
   - Copy the example environment file:
     ```bash
     cp .env.example .env
     ```
   - Edit the `.env` file and fill in your configuration values:
     - `MONGODB_URI`: Your MongoDB connection string
     - `JWT_SECRET`: A secure random string for JWT token signing
     - `GEMINI_API_KEY`: Your Google Gemini AI API key
     - `PORT`: The port number for the server (default: 3000)
     - Other optional configurations as needed

   Required Environment Variables:
   ```
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   GEMINI_API_KEY=your_gemini_api_key
   PORT=3000
   ```

   Optional Environment Variables:
   ```
   NODE_ENV=development
   FRONTEND_URL=http://localhost:8080
   SESSION_SECRET=your_session_secret
   LOG_LEVEL=debug
   ```

## Running the Application

1. Start the development server:
```bash
npm start
```

2. For development with auto-reload:
```bash
npm run dev
```

3. To run just the frontend:
```bash
npm run frontend
```

## Project Structure

```
ai-friend/
├── server/           # Backend server code
├── js/              # Frontend JavaScript files
├── css/             # Stylesheets
├── images/          # Image assets
├── .env             # Environment variables (not in git)
├── .env.example     # Example environment variables
├── start.js         # Application entry point
├── config.js        # Configuration file
└── package.json     # Project dependencies
```

## API Documentation

### Authentication Endpoints
- POST /api/auth/register - User registration
- POST /api/auth/login - User login
- GET /api/auth/verify - Verify user token

### Chat Endpoints
- POST /api/chat/send - Send message to AI
- GET /api/chat/history - Get chat history

### Journal Endpoints
- POST /api/journal/entry - Create journal entry
- GET /api/journal/entries - Get journal entries

### Mood Tracking Endpoints
- POST /api/mood/track - Track mood
- GET /api/mood/history - Get mood history

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Security

- All sensitive data is stored securely using encryption
- User authentication is handled using JWT tokens
- API keys and secrets are stored in environment variables
- Regular security audits are performed

## License

This project is licensed under the ISC License - see the LICENSE file for details.

## Support

For support, please open an issue in the GitHub repository or contact the maintainers.

## Acknowledgments

- Google Gemini AI for providing the AI capabilities
- Express.js team for the web framework
- MongoDB for the database solution 
