# Autonomous Job Application Tracker

A full-stack web application automating job application tracking via AI-powered email analysis.  Streamline your job search and effortlessly monitor your application progress.

## Description

The Autonomous Job Application Tracker is designed to revolutionize the job application process.  By leveraging the power of machine learning and cloud-based email processing, this application automatically tracks your job applications, eliminating manual data entry and keeping you informed of updates in real-time.  Built using a robust full-stack architecture, it provides a seamless and efficient way to manage your job search.

## Key Features

* **AI-Powered Email Analysis:** A custom machine learning model (Python, SpaCy) analyzes your emails to identify job application-related messages and automatically classify their status (Applied, Under Review, Interview, Accepted, Rejected).

* **Automated Email Processing:** Securely integrates with your Gmail account (Google OAuth2) to automatically process incoming emails.

* **Dynamic Database Updates:**  New applications are added and existing application statuses are updated automatically based on email content.

* **Centralized Web Interface:**  A user-friendly interface (Next.js, React, TypeScript) provides a single dashboard to monitor all your job applications.

* **Robust Backend:**  Powered by Node.js, Express, and a SQL database for secure and efficient data management.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

* Node.js and npm (or yarn)
* Python 3.x and pip
* A Google Cloud Platform (GCP) project with the Gmail API enabled.  (See [Google Cloud Setup](./docs/gcp_setup.md) for detailed instructions)
* PostgreSQL (or your preferred SQL database)

### Installation

1. **Clone the repository:**
   ```bash
   git clone <repository_url>
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd ../frontend
   npm install
   ```

4. **Setup the database:**  Follow the instructions in [Database Setup](./docs/database_setup.md).

5. **Configure environment variables:** Create a `.env` file in both the `backend` and `frontend` directories with the necessary credentials (API keys, database connection strings, etc.).  See the `.env.example` files for guidance.

### Running the Application

1. **Start the backend:**
   ```bash
   cd backend
   npm start
   ```

2. **Start the frontend:**
   ```bash
   cd ../frontend
   npm run dev
   ```

The application should now be accessible at `http://localhost:3000` (or the port specified in your frontend `.env` file).
