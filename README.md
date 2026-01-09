# Project Setup Instructions

I have prepared the necessary configuration to run the LIFENET project on your device.

## Prerequisites
- **Python**: Make sure Python is installed and added to your system PATH.

## Automatic Setup
I have created a `setup.bat` file that will automatically:
1. Create a virtual environment (`venv`).
2. Install all required dependencies from `requirements.txt`.
3. Apply database migrations.

**To start:**
1. Double-click `setup.bat` in this folder.
2. Wait for the process to complete.

## Running the Server
Once setup is complete, you can start the server by double-clicking `run_server.bat`.

## Manual Setup (Alternative)
If you prefer to run commands manually:

1. Open a terminal in this directory.
2. Create a virtual environment:
   ```cmd
   python -m venv venv
   ```
3. Activate the environment:
   ```cmd
   venv\Scripts\activate
   ```
4. Install dependencies:
   ```cmd
   pip install -r requirements.txt
   ```
5. Run migrations:
   ```cmd
   python manage.py migrate
   ```
6. Start the server:
   ```cmd
   python manage.py runserver
   ```
