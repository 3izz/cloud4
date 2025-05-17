# Link Library

A cloud-based application for managing and categorizing links with role-based access control.

## Features

- User authentication and role-based access control
- Private link library for each user
- Automatic link classification (safe/unsafe)
- Background music feature
- Built-in chatbot assistance
- Responsive web interface

## Setup Instructions

1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file in the root directory with the following variables:
```
SECRET_KEY=your_secret_key
DATABASE_URL=sqlite:///link_library.db
```

4. Initialize the database:
```bash
python init_db.py
```

5. Run the application:
```bash
python app.py
```

The application will be available at `http://localhost:5000`

## Security Features

- Password hashing using bcrypt
- JWT-based authentication
- Role-based access control
- Secure link validation
- XSS protection

## Project Structure

```
link_library/
├── app/
│   ├── __init__.py
│   ├── models/
│   ├── routes/
│   ├── static/
│   └── templates/
├── config.py
├── requirements.txt
└── README.md
``` 