# My Portfolio Website

This is a simple, responsive portfolio website built with Flask and Tailwind CSS.

## Features

* **Clean Design:** Modern and minimalist aesthetic.
* **Responsive:** Adapts to various screen sizes (mobile, tablet, desktop).
* **Sections:** Home (Hero), About Me, Skills, Projects, and Contact.
* **Easy to Customize:** Built with Flask templates and Tailwind CSS for quick modifications.

## Project Structure
myportfolio/
│
├── static/
│   ├── css/
│   │   └── style.css          # Custom CSS (mainly for fonts/overrides)
│   └── images/
│       └── yourphoto.jpg      # Placeholder for your profile photo
│
├── templates/
│   ├── index.html             # Main content for the home page
│   └── layout.html            # Base template with common structure and Tailwind CSS
│
├── app.py                     # Flask application
├── requirements.txt           # Python dependencies
└── README.md                  # Project README file


## Setup and Run

Follow these steps to get the project up and running on your local machine or Codespaces:

1.  **Clone the repository (if applicable) or navigate to your project directory.**
    If you're in Codespaces and just created the files, you're already in the `myportfolio` directory.

2.  **Create a Python Virtual Environment (Recommended):**
    ```bash
    python3 -m venv venv
    ```

3.  **Activate the Virtual Environment:**
    * **On macOS/Linux:**
        ```bash
        source venv/bin/activate
        ```
    * **On Windows (Command Prompt):**
        ```bash
        venv\Scripts\activate.bat
        ```
    * **On Windows (PowerShell):**
        ```powershell
        .\venv\Scripts\Activate.ps1
        ```

4.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

5.  **Run the Flask Application:**
    ```bash
    python app.py
    ```

    The application will typically run on `http://127.0.0.1:5000/` (or a similar address provided by Codespaces). Open this URL in your web browser.

6.  **Accessing Sections:** You can directly navigate to specific sections of the portfolio by appending the section ID to the URL (e.g., `http://127.0.0.1:5000/#skills` to go directly to the Skills section).

## Customization

## Customization

* **Your Photo:** Replace `static/images/yourphoto.jpg` with your actual profile picture. Make sure it's a square or circular image for best results.
* **Content:** Edit the text in `templates/index.html` to reflect your "About Me," "Skills," "Projects," and "Contact" details.
* **Links:** Update the social media links in `templates/layout.html` and project links in `templates/index.html` with your own.
* **Colors/Fonts:** Modify Tailwind CSS classes in `templates/layout.html` and `templates/index.html` to change the color scheme or font if desired. Refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs) for available classes.
* **New Pages:** To add more pages, create new HTML files in the `templates` directory and define new routes in `app.py` to render them.
