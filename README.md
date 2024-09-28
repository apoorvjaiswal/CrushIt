# Dating Application

A full-featured dating application built with **React** for the frontend and **.NET MVC** for the backend, offering a seamless experience for users to connect, match, and chat with potential partners.

## Features
- **User Authentication**: Secure sign-up and login with email verification.
- **Profile Management**: Users can create and update their profiles with pictures and personal information.
- **Matchmaking**: Intelligent matching based on user preferences and location.
- **Swipe Functionality**: Intuitive swipe interface for liking or passing on profiles.
- **Real-Time Chat**: Instant messaging with matched users.
- **Search Filters**: Filter users based on age, location, and interests.
- **Notifications**: Receive notifications for new matches and messages.

## Tech Stack
- **Frontend**: React (for responsive UI and client-side rendering)
- **Backend**: .NET MVC (for business logic, authentication, and matchmaking algorithms)
- **Database**: SQL Server (for storing user profiles, matches, and chat history)
- **Real-Time Communication**: SignalR (for real-time chat)

## Requirements
- **Node.js** (for React frontend)
- **.NET SDK** (for MVC backend)
- **SQL Server** (for the database)
- **Visual Studio** or **VS Code** (for development environment)

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/dating-app.git
cd dating-app
```

### 2. Install Frontend Dependencies
Navigate to the frontend directory and install the React dependencies:
```bash
cd frontend
npm install
```

### 3. Set Up .NET MVC Backend
1. Navigate to the backend directory.
```bash
cd backend
```
2. Restore the .NET project dependencies:
```bash
dotnet restore
```

### 4. Configure SQL Server Database
1. Set up a SQL Server instance.
2. Create a database for the application and update the connection string in the `appsettings.json` file.

```json
// Inside appsettings.json
"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER;Database=YOUR_DATABASE;Trusted_Connection=True;"
}
```

3. Apply migrations to set up the database schema:
```bash
dotnet ef database update
```

### 5. Run the Application

#### Run the Backend (.NET MVC)
```bash
cd backend
dotnet run
```

#### Run the Frontend (React)
In a separate terminal, start the React development server:
```bash
cd frontend
npm start
```

### 6. Access the Application
Once both the backend and frontend are running, open your browser and visit:
```
http://localhost:3000
```

## API Documentation
Your .NET backend exposes the following key API endpoints:
- **User Authentication**: `/api/auth/login`, `/api/auth/register`
- **Profile Management**: `/api/profile`
- **Matchmaking**: `/api/match`
- **Chat**: `/api/chat`

Refer to the `backend` folder for detailed API documentation and usage.

## Example Usage
1. Sign up with your email and create a profile.
2. Browse through potential matches and swipe right to like a profile.
3. Once matched, start chatting with your connections in real time.
4. Update your profile and search for users using filters.

## Contributing
Contributions are welcome! If you want to add features or fix bugs, feel free to fork the repo and submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.
