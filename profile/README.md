# qRate - Queen's Course Rating Platform

## About qRate

qRate is a comprehensive course and professor rating platform designed exclusively for Queen's University students. Built by students, for students, qRate empowers the Queen's community to make informed academic decisions through authentic peer reviews and comprehensive course data.

### What qRate Does

- **Course Discovery**: Browse and search through Queen's University courses with detailed information, ratings, and student reviews
- **Professor Insights**: Access ratings and reviews for professors across all faculties at Queen's
- **Authentic Reviews**: Read and submit genuine student experiences with courses and instructors
- **Academic Planning**: Make informed course selection decisions based on peer feedback about difficulty, usefulness, workload, and teaching quality
- **Community-Driven**: Built and maintained by Queen's students using real student experiences

### Key Features

- **Comprehensive Course Database**: Complete course catalog with prerequisites, descriptions, and offering terms
- **Multi-dimensional Ratings**: Courses rated on overall quality, difficulty, usefulness, workload, and teaching quality
- **Professor Profiles**: Detailed professor pages with ratings for helpfulness, clarity, and difficulty
- **Authenticated Reviews**: Queen's-only access using @queensu.ca email verification
- **Advanced Filtering**: Search and filter by faculty, department, rating, and more
- **Responsive Design**: Optimized for desktop and mobile usage

## Technology Stack

### Frontend
- **Framework**: React 18 with TypeScript
- **Routing**: React Router v6
- **Styling**: Tailwind CSS with shadcn/ui components
- **State Management**: React hooks (useState, useEffect, custom hooks)
- **HTTP Client**: Axios for API communication
- **Build Tool**: Vite
- **Deployment**: Hosted on modern web hosting platform

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JWT-based auth system
- **Email Verification**: Integrated email verification for @queensu.ca accounts
- **API Architecture**: RESTful API design
- **Deployment**: Azure Web Services

### Database Schema
- **Users Collection**: Student accounts with email verification
- **Courses Collection**: Complete Queen's course catalog with metadata
- **Reviews Collection**: Student course reviews with ratings and comments
- **Professors Collection**: Faculty information and aggregated ratings
- **Professor Reviews Collection**: Professor-specific student feedback

## Development Team

**Core Development Team (Class of 2026)**
- **Nathan Daniel** - Full-stack development, AI integration, hardware architecture
- **Lucas Srigley** - Backend specialist, database architecture, API development  
- **Jamie Bell** - Data systems, rating algorithms, review aggregation
- **Nolan Steed** - Data optimization, algorithm development, system performance

All team members are Computer Engineering students at Queen's University.

## Getting Started

### Prerequisites
- Node.js 18+
- MongoDB instance
- Queen's University email address (@queensu.ca)

### Frontend Setup
```bash
git clone https://github.com/qrate-org/qrate-frontend
cd qrate-frontend
npm install
npm run dev
```

### Backend Setup
```bash
git clone https://github.com/qrate-org/qrate-backend
cd qrate-backend
npm install
npm start
```

### Environment Variables
- `MONGODB_URI` - MongoDB connection string
- `JWT_SECRET` - Secret key for JWT tokens
- `EMAIL_SERVICE` - Email service configuration
- `FRONTEND_URL` - Frontend application URL

## API Endpoints

### Courses
- `GET /api/v1/courses` - Browse courses with pagination
- `GET /api/v1/courses/:id` - Get specific course details
- `POST /api/v1/reviews/new` - Submit course review

### Professors  
- `GET /api/v1/professors` - Browse professors
- `GET /api/v1/professor-reviews/search` - Get professor reviews
- `POST /api/v1/professor-reviews/new` - Submit professor review

### Authentication
- `POST /api/v1/auth/register` - Create account
- `POST /api/v1/auth/login` - User login
- `GET /api/v1/auth/verify` - Email verification

- Respect student privacy and data security

## Privacy & Security

- Email verification required for all accounts
- No personal information shared beyond username
- Reviews are anonymous to protect student privacy
- Data secured with industry-standard practices
- Compliant with Canadian privacy regulations

**Built with ❤️ by Queen's students, for Queen's students**

*Not affiliated with Queen's University. An independent student-led initiative.*
