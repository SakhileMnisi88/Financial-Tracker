# Financial-Tracker💵

A modern, full-stack web application for tracking and managing personal finances.

## Tech Stack

### Frontend
- **React** - UI library for building interactive interfaces
- **TailwindCSS** - Utility-first CSS framework for styling
- **Vercel** (optional) - Deployment platform

### Backend
- **FastAPI** - High-performance Python web framework
- **PyJWT** - JWT token authentication
- **Render/Fly.io** (optional) - Backend hosting

### Database
- **PostgreSQL** - Reliable relational database for finance data
- **SQLAlchemy** - Python ORM for database operations
- **Alembic** - Database migration tool

### Documentation
- **Swagger** - Auto-generated API documentation (built into FastAPI)

## Features

- 🔐 Secure authentication with JWT tokens
- 💰 Track income and expenses
- 📊 View financial summaries and reports
- 🗄️ Persistent data storage with PostgreSQL
- 📱 Clean, responsive UI
- 📖 Interactive API documentation

## Getting Started

### Prerequisites
- Python 3.8+
- Node.js 16+
- PostgreSQL 12+

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd finance-tracker
```

2. **Backend Setup**
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

3. **Database Setup**
```bash
# Create a PostgreSQL database
createdb finance_tracker

# Run migrations
alembic upgrade head
```

4. **Frontend Setup**
```bash
cd frontend
npm install
```

### Running the Application

1. **Start the backend**
```bash
cd backend
uvicorn main:app --reload
```
The API will be available at `http://localhost:8000`
API docs at `http://localhost:8000/docs`

2. **Start the frontend**
```bash
cd frontend
npm run dev
```
The app will be available at `http://localhost:3000`

## Environment Variables

Create `.env` files in both frontend and backend directories:

**Backend `.env`**
```
DATABASE_URL=postgresql://user:password@localhost/finance_tracker
SECRET_KEY=your-secret-key-here
```

**Frontend `.env`**
```
REACT_APP_API_URL=http://localhost:8000
```

## Project Structure

```
finance-tracker/
├── frontend/          # React frontend
│   ├── src/
│   └── public/
├── backend/           # FastAPI backend
│   ├── models/
│   ├── routes/
│   └── main.py
└── README.md
```

## API Documentation

Once the backend is running, visit `http://localhost:8000/docs` for interactive API documentation powered by Swagger.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License - feel free to use this project for your own purposes.
