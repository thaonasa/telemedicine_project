# Telemedicine Project

A modern telemedicine platform built with FastAPI/React and containerized with Docker.

## Project Structure

```
telemedicine-project/
├── backend/                  # FastAPI backend
├── frontend/                 # React frontend
├── nginx/                    # Reverse proxy configuration
├── db/                      # Database initialization scripts
├── docker-compose.yml       # Docker compose configuration
├── .env                     # Environment variables
└── .github/workflows/       # CI/CD pipelines
```

## Prerequisites

- Docker and Docker Compose
- Node.js (for local frontend development)
- Python 3.8+ (for local backend development)

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/telemedicine-project.git
   cd telemedicine-project
   ```

2. Create and configure your `.env` file:
   ```bash
   cp .env.example .env
   # Edit .env with your configurations
   ```

3. Start the application:
   ```bash
   docker-compose up -d
   ```

4. Access the application:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:8000/docs
   - Admin panel: http://localhost:8000/admin

## Development

### Backend Development
```bash
cd backend
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Frontend Development
```bash
cd frontend
npm install
npm start
```

## Testing

```bash
# Backend tests
cd backend
pytest

# Frontend tests
cd frontend
npm test
```

## Deployment

The application uses GitHub Actions for CI/CD. See `.github/workflows` for the pipeline configurations.

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
