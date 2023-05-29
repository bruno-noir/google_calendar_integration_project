# Google Calendar API OAuth 2.0 Integration with Django Rest Framework

This project demonstrates the integration of Google Calendar API with Django Rest Framework using OAuth 2.0. It provides API endpoints to authenticate users and retrieve their calendar events.

## Getting Started

To run this project on your local machine, follow these steps:

### Prerequisites

- Python (version 3.6 or higher)
- pip (package installer for Python)
- Virtual environment (optional but recommended)

### Installation

1. Clone the repository to your local machine:
   ```sh
   git clone https://github.com/your-username/google-calendar-integration.git
2. Navigate to the project directory:
   ```sh
   cd google-calendar-integration
3. (Optional) Create and activate a virtual environment:
   ```sh
   python -m venv myenv
   source myenv/bin/activate
4. Install the required packages:
   ```sh
   pip install -r requirements.txt
   
## Configuration

1. Create a Google Cloud project and enable the Google Calendar API.
2. Obtain the OAuth 2.0 client ID and client secret for your project.
3. Save the client ID and client secret in a secure manner.

### Setting up Google Account Credentials

1. In the project directory, create a new file named `credentials.json`.
2. Open the `credentials.json` file and paste the following content:
   ```json
   {
   "GOOGLE_CALENDAR_CLIENT_ID": "YOUR_CLIENT_ID",
   "GOOGLE_CALENDAR_CLIENT_SECRET": "YOUR_CLIENT_SECRET"
   }
3. Replace '"YOUR_CLIENT_ID"' and '"YOUR_CLIENT_SECRET"' with the actual values obtained from the Google Cloud Console.

### Setting up Google Account Credentials

1. Apply the database migrations:
   ```json
   python manage.py migrate

### Usage

1. Start the Django development server:
   ```json
   python manage.py runserver
2. Access the API endpoints:
    Initiate the OAuth process by visiting: 'http://localhost:8000/rest/v1/calendar/init/'. This will prompt the user for their credentials.
    Handle the redirect request from Google by visiting: 'http://localhost:8000/rest/v1/calendar/redirect/'. This will obtain the access token and retrieve the user's calendar events.

> **Note**: Before accessing these endpoints, make sure you have completed the configuration steps mentioned above and have the necessary Google Account credentials saved in the project directory.
