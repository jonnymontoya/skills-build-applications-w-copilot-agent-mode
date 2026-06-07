# OctoFit Tracker Backend

A Node.js + Express + TypeScript backend for the OctoFit Tracker application with MongoDB data access via Mongoose.

## Configuration

- **Frontend URL**: http://localhost:5173
- **Backend Server**: http://localhost:8000
- **MongoDB**: mongodb://localhost:27017 (default)
- **Database Name**: octofit

## Setup

### Environment Variables

Create a `.env` file in the backend directory (optional):

```
PORT=8000
MONGODB_URI=mongodb://localhost:27017/octofit
```

## Available Scripts

- `npm run dev` - Start the development server with hot reload (nodemon + ts-node)
- `npm run build` - Compile TypeScript to JavaScript
- `npm start` - Run the built application

## Project Structure

```
backend/
├── src/
│   └── index.ts          # Main server entry point
├── build/                # Compiled JavaScript (generated)
├── package.json
├── tsconfig.json         # TypeScript configuration
└── README.md
```

## Dependencies

### Production
- **express**: Web framework for Node.js
- **mongoose**: MongoDB object modeling and validation

### Development
- **typescript**: TypeScript compiler
- **ts-node**: Run TypeScript directly
- **nodemon**: Auto-reload on file changes
- **@types/node**: Node.js type definitions
- **@types/express**: Express type definitions

## API Endpoints

- `GET /` - API information
- `GET /health` - Health check endpoint

## Getting Started

1. Ensure MongoDB is running on port 27017
2. Install dependencies: `npm install`
3. Start development server: `npm run dev`
4. Server will be available at http://localhost:8000
