THIS IS MY BENMORE TECHNOLOGIES LTD ASSESSMENT TO BUILD A FUNCTIONAL TASK MANAGEMENT APP

## Setting Up and Running the Task Management App

This guide explains how to set up and run the Django task management application locally on your development machine.

**Prerequisites:**

* **Python 3.x:** Download and install Python from [https://www.python.org/downloads/](https://www.python.org/downloads/). Ensure you have the appropriate version for your operating system.
* **pip:** pip is the package installer for Python. It usually comes bundled with Python. You can verify its installation by running `pip --version` in your terminal.
* **Git:** Download and install Git from [https://git-scm.com/downloads](https://git-scm.com/downloads) if you don't have it already.
* **Code Editor or IDE:** Choose a code editor or IDE of your preference, such as Visual Studio Code, PyCharm, or Sublime Text.

**Steps:**

1. **Clone the Repository:**

   Open your terminal and navigate to the desired directory where you want to set up the project. 
   Run the following command, replacing `<URL>` with the actual URL of your cloned GitHub repository:

   ```bash
   git clone <URL>
   ```

2. **Create a Virtual Environment (Recommended):**

   - A virtual environment isolates project dependencies and avoids conflicts with other Python installations.
   - Use the `venv` module to create a virtual environment:

   ```bash
   python -m venv venv
   ```

   - Activate the virtual environment (commands differ slightly based on OS):

      - **Windows:** `venv\Scripts\activate`
      - **macOS/Linux:** `source venv/bin/activate`

3. **Install Dependencies:**

   - Inside the activated virtual environment, navigate to the project's root directory.
   - Run the following command to install the required Python packages listed in the project's `requirements.txt` file:

   ```bash
   pip install -r requirements.txt
   ```

4. **Database Setup:**

   - The project likely uses a database to store task data. You'll need to configure the database settings in your Django project's `settings.py` file. This might involve:
      - Specifying the database engine (e.g., `DATABASES['default']['ENGINE'] = 'django.db.backends.postgresql'`)
      - Setting up database credentials (username, password, hostname, port)
   - Follow the project's specific instructions or Django documentation for database configuration: [https://docs.djangoproject.com/en/5.0/](https://docs.djangoproject.com/en/5.0/)

   - **Optional:** If the project includes database migrations, you can run them using the command:

   ```bash
   python manage.py migrate
   ```

5. **Run the Development Server:**

   - Make sure your virtual environment is activated.
   - Run the following command to start the Django development server:

   ```bash
   python manage.py runserver
   ```

   - This will typically start the server on `http://127.0.0.1:8000/` by default. Open this URL in your web browser to access the application.

**Additional Notes:**

* The provided instructions are general guidelines. The specific steps might vary slightly depending on the project's configuration.
* Consult the project's README file or documentation for any additional setup instructions or environment variables required.
* Consider creating a `.env` file to manage sensitive environment variables like database credentials (refer to Django documentation for details).

By following these steps, you should be able to set up and run the Django task management application locally on your development machine. If you encounter any issues during the setup process, refer to the project's documentation or search online for specific error messages.
