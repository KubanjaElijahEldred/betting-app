# Sports Betting Dashboard

A modern sports betting and fantasy football dashboard built with React, Java Spring Boot, and MongoDB.

## Features

- 🔐 **Authentication System** - JWT-based login and signup
- 🌓 **Dark/Light Theme** - Toggle between themes
- ⚽ **Player Statistics** - Comprehensive player data and rankings
- 📊 **Dashboard** - Live matches, statistics, and fantasy team management
- 🏆 **Multiple Pages** - Players, Matches, Leagues, Statistics, Betting, Profile
- 📱 **Responsive Design** - Modern UI with TailwindCSS

## Tech Stack

### Frontend
- React 18 with TypeScript
- TailwindCSS for styling
- Context API for state management
- JWT authentication
- Responsive design

### Backend
- Java 17
- Spring Boot 3.1.5
- Spring Security with JWT
- MongoDB integration
- RESTful API design

### Database
- MongoDB for data storage
- Sample player data included

## Getting Started

### Prerequisites
- Node.js 16+
- Java 17+
- MongoDB (local or cloud)
- Maven

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd "Betting App"
   ```

2. **Setup Backend**
   ```bash
   cd backend
   mvn clean install
   mvn spring-boot:run
   ```
   Backend will run on `http://localhost:8080`

3. **Setup Frontend**
   ```bash
   cd frontend
   npm install
   npm start
   ```
   Frontend will run on `http://localhost:3000`

4. **MongoDB Setup**
   - Install MongoDB locally or use MongoDB Atlas
   - Update `application.yml` with your MongoDB connection string
   - Sample data will be automatically loaded on first run

## API Endpoints

### Authentication
- `POST /api/auth/signin` - User login
- `POST /api/auth/signup` - User registration

### Players
- `GET /api/players` - Get all players
- `GET /api/players/top` - Get top 10 players by points
- `GET /api/players/{id}` - Get player by ID
- `GET /api/players/team/{team}` - Get players by team
- `GET /api/players/position/{position}` - Get players by position

## Demo Credentials

For testing purposes, you can use:
- **Email**: demo@example.com
- **Password**: password

Or create a new account using the signup form.

## Project Structure

```
Betting App/
├── frontend/                 # React frontend
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── contexts/        # Context providers
│   │   └── ...
│   └── package.json
├── backend/                 # Spring Boot backend
│   ├── src/main/java/
│   │   └── com/sportsbet/backend/
│   │       ├── controller/  # REST controllers
│   │       ├── model/       # Data models
│   │       ├── repository/  # Data repositories
│   │       ├── service/     # Business logic
│   │       ├── security/    # Security configuration
│   │       └── dto/         # Data transfer objects
│   └── pom.xml
└── README.md
```

## Features Implementation

### ✅ Completed
- Authentication system (login/signup)
- Dark/light theme toggle
- Dashboard with player statistics
- Navigation between pages
- Modern UI matching the design requirements
- Backend API with JWT security
- MongoDB integration
- Sample data initialization

### 🚧 Future Enhancements
- Real-time match data
- Betting functionality
- Advanced statistics
- User profile management
- Fantasy team builder
- Live chat/notifications

## Screenshots

The application implements the exact dashboard design from the provided images with:
- Modern dark theme with blue/purple gradients
- Player statistics and rankings
- Live match data display
- Clean navigation sidebar
- Responsive card layouts

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License.
