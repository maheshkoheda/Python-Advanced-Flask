# Flask Advanced To-Do Application

A simple to-do application built using Flask, SQLAlchemy, and SQLite. The app allows users to create, update, delete, and view tasks.

## Features

- **Add Tasks**: Users can add new tasks with descriptions.
- **View Tasks**: Displays all tasks in the order they were created.
- **Update Tasks**: Edit the description of a task.
- **Delete Tasks**: Remove tasks from the list.
- **Database**: Tasks are stored persistently using SQLite.

## Project Structure

```
Flask-Advanced/
├── app.py             # Main application logic
├── instance/
│   └── test.db        # SQLite database
├── static/            # Static assets (e.g., CSS, JS)
├── templates/
│   ├── base.html      # Base template
│   ├── index.html     # Homepage template
│   └── update.html    # Task update template
├── env/               # Virtual environment (if used)
├── .gitignore         # Git ignore file
└── __pycache__/       # Compiled Python files
```

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Flask-Advanced
   ```

2. Set up a virtual environment (optional but recommended):
   ```bash
   python -m venv env
   source env/bin/activate   # For Linux/macOS
   env\Scripts\activate      # For Windows
   ```

3. Install the dependencies:
   ```bash
   pip install flask flask-sqlalchemy
   ```

4. Ensure the `instance` folder exists for the database:
   ```bash
   mkdir instance
   ```

## Usage

1. Run the application:
   ```bash
   python app.py
   ```

2. Open your browser and navigate to `http://127.0.0.1:5000`.

## Templates Overview

- **`index.html`**: Lists all tasks with options to delete or update.
- **`update.html`**: Form to update task details.
- **`base.html`**: Base layout for consistent styling.

## Testing the Application

1. **Add a Task**:
   - Go to the homepage (`/`).
   - Fill in the task input field and click "Add Task."

2. **Delete a Task**:
   - Click the "Delete" button next to the task.

3. **Update a Task**:
   - Click the "Update" button next to the task.
   - Edit the content in the form and submit.

4. **Database Check**:
   - The SQLite database (`test.db`) stores all tasks persistently.

## Notes

- The app uses a `test.db` SQLite database located in the `instance` folder.
- Flask's debug mode is enabled for development.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

