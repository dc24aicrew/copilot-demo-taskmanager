# Task Manager Demo App

🚀 **Demo repository for GitHub Copilot Coding Agent showcases**

This is a comprehensive Task Management application built with Node.js, Express, and MongoDB. It's designed to demonstrate various GitHub Copilot capabilities through real-world scenarios.

## 📋 Features

- **User Authentication & Authorization**
  - JWT-based authentication
  - Role-based access control (User, Admin, Manager)
  - Secure password hashing
  - Profile management

- **Task Management**
  - Create, read, update, delete tasks
  - Task assignment and ownership
  - Priority levels (Low, Medium, High, Urgent)
  - Status tracking (Todo, In Progress, Review, Completed)
  - Categories and tags
  - Due dates and time tracking
  - Comments and attachments

- **Advanced Features**
  - Search and filtering
  - Pagination
  - Data validation
  - Error handling
  - Security middleware
  - Rate limiting

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JWT (JSON Web Tokens)
- **Validation**: Joi, express-validator
- **Security**: Helmet, CORS, bcryptjs
- **Testing**: Jest, Supertest
- **Development**: Nodemon, ESLint

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/dc24aicrew/copilot-demo-taskmanager.git
   cd copilot-demo-taskmanager
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

4. **Start MongoDB**
   ```bash
   # Using Docker
   docker run -d -p 27017:27017 --name mongodb mongo:latest
   
   # Or use MongoDB Atlas (cloud)
   ```

5. **Run the application**
   ```bash
   # Development mode
   npm run dev
   
   # Production mode
   npm start
   ```

## 📚 API Documentation

### Authentication Endpoints

- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/me` - Get current user profile
- `PUT /api/auth/profile` - Update user profile

### Task Endpoints

- `GET /api/tasks` - Get tasks with filtering and pagination
- `POST /api/tasks` - Create new task
- `GET /api/tasks/:id` - Get single task
- `PUT /api/tasks/:id` - Update task
- `DELETE /api/tasks/:id` - Delete task
- `POST /api/tasks/:id/comments` - Add comment to task

### User Endpoints

- `GET /api/users` - Get users list
- `GET /api/users/:id` - Get user profile

## 🎯 GitHub Copilot Demo Scenarios

This repository is specifically designed to showcase GitHub Copilot capabilities:

### 1. **Code Review & Bug Detection**
- Security vulnerabilities (SQL injection, XSS)
- Logic errors and edge cases
- Code style and best practices
- Performance optimizations

### 2. **Feature Implementation**
- Real-time notifications
- File upload functionality
- Advanced search and filtering
- Analytics dashboard
- Email integration

### 3. **Testing & Quality**
- Unit tests for models and controllers
- Integration tests for API endpoints
- Test data generation
- Code coverage improvements

### 4. **Documentation & Refactoring**
- API documentation generation
- Code comments and JSDoc
- Legacy code modernization
- Performance optimizations

### 5. **DevOps & Deployment**
- Docker containerization
- CI/CD pipeline setup
- Environment configuration
- Monitoring and logging

## 🔧 Development

### Available Scripts

```bash
npm run dev        # Start development server with nodemon
npm start          # Start production server
npm test           # Run tests
npm run test:watch # Run tests in watch mode
npm run lint       # Run ESLint
npm run lint:fix   # Fix ESLint errors
```

### Project Structure

```
├── models/          # Database models
│   ├── User.js     # User model with authentication
│   └── Task.js     # Task model with relationships
├── routes/          # API routes
│   ├── auth.js     # Authentication routes
│   ├── tasks.js    # Task management routes
│   └── users.js    # User management routes
├── middleware/      # Custom middleware
│   └── auth.js     # JWT authentication middleware
├── tests/          # Test files (to be created)
├── docs/           # Documentation (to be created)
└── server.js       # Application entry point
```

## 🎪 Demo Instructions

### For Demo Leaders:

1. **Preparation**
   - Fork this repository
   - Set up local development environment
   - Create demo issues with specific requirements

2. **Live Demo Flow**
   - Start with a simple feature request issue
   - Assign Copilot to the issue
   - Show the automatic PR creation
   - Review and merge the changes
   - Demonstrate code review capabilities

3. **Advanced Scenarios**
   - Complex feature implementation
   - Bug fixing and security improvements
   - Test generation and documentation

## 🐛 Known Issues (For Demo Purposes)

Some intentional issues are included for Copilot demonstrations:

- Missing input validation in some endpoints
- Potential security vulnerabilities
- Missing error handling in certain scenarios
- Incomplete test coverage
- Missing API documentation

## 📝 License

MIT License - feel free to use this for your own Copilot demonstrations!

## 🤝 Contributing

This is a demo repository, but feel free to:
- Report issues
- Suggest improvements
- Create demo scenarios
- Add test cases

---

**Happy Coding with GitHub Copilot! 🚁✨**