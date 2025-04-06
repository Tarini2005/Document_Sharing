# Web App

Site for students to share course materials and help those taking the same class later.

## Steps necessary to run the software

1. Prerequisites:
   - Python 3.11 or higher
   - MongoDB Atlas account

2. Clone the repository and set up virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   ```bash
   cp .env.example .env
   ```
   Or create a `.env` file in the root directory with the following content:
   ```
   MONGO_URI=your_mongodb_connection_string
   SECRET_KEY=your_secret_key
   DEBUG=True
   UPLOAD_FOLDER=./uploads
   MAX_CONTENT_LENGTH=16777216
   ```

5. Run the application:
   ```bash
   python app.py
   ```

6. Access the application at `http://localhost:5001`

