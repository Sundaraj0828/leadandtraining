# LeadAndTraining Management System 🚀

LeadAndTraining is a high-performance RESTful application designed to streamline the lifecycle of student leads and vocational training programs. It provides a centralized backend to manage prospective client data, track training progress, and automate the conversion of leads into active participants.

## 🛠️ Tech Stack

* Backend: Python 3.10+ with Flask Framework
* API Architecture: RESTful Design
* Database: MongoDB (NoSQL for flexible data modeling)
* Authentication: JWT (JSON Web Tokens) via Flask-JWT-Extended
* Configuration: `python-dotenv` for secure environment variables
* Validation: Marshmallow (suggested for request/response schema)


## ✨ Key Features

* Lead Lifecycle Tracking: Manage leads from "New" to "Enrolled" or "Closed."
* Training Module Management: Create, update, and assign training sessions to specific leads.
* Secure API Access: Protected endpoints ensuring only authorized admins can modify data.
* Scalable Architecture: Built with a decoupled frontend-ready approach.
* Dynamic Queries: Leverages MongoDB’s flexibility for complex lead filtering.


## 🚀 Getting Started

### 1. Prerequisites
* Python 3.10 or higher
* MongoDB installed and running (locally or Atlas)

### 2. Installation
Clone the repository and navigate to the project directory:
```bash
git clone https://github.com/Sundaraj0828/leadandtraining.git
cd leadandtraining
```

### 3. Environment Setup
Create a `.env` file in the root directory to protect your credentials:
```env
FLASK_APP=app.py
FLASK_ENV=development
MONGO_URI=mongodb://localhost:27017/lead_training_db
JWT_SECRET_KEY=your_random_secure_string_here
```

### 4. Install Dependencies
```bash
pip install -r requirements.txt
```

### 5. Run the Application
```bash
flask run
```
The server will start at `http://127.0.0.1:5000/`.



## 🔗 API Documentation

| Method | Endpoint | Description | Auth Required |
| :--- | :--- | :--- | :--- |
| GET | `/api/leads` | Retrieve all leads | Yes |
| POST | `/api/leads` | Create a new lead | Yes |
| GET | `/api/leads/<id>` | Get specific lead details | Yes |
| PUT | `/api/training/<id>` | Update training status | Yes |
| POST | `/api/auth/login` | Obtain JWT access token | No |


## 📁 Project Structure
```text
├── app/
│   ├── models/          # MongoDB Schemas
│   ├── routes/          # REST API Endpoints
│   ├── utils/           # Helpers & Auth decorators
│   └── __init__.py      # Flask app factory
├── .env                 # Environment variables (Hidden)
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```



## 📄 License
Distributed under the MIT License. See `LICENSE` for more information.



Developed with ❤️ by [L.C. Sundaraj/Sundaraj0828]
