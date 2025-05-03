# Git Practice App

A simple Flask web application for practicing Git collaboration.

## Setup Instructions




1. Clone this repository:
```bash
git clone <repository-url>
cd git_learner
```

2. Create a virtual environment:
```bash
python -m venv venv
```

3. Activate the virtual environment:
- Windows:
```bash
venv\Scripts\activate
```
- macOS/Linux:
```bash
source venv/bin/activate
```

4. Install dependencies:
```bash
pip install -r requirements.txt
```

5. Run the application:
```bash
python app.py
```

6. Open your browser and visit: `http://localhost:5000`

## How to Add New Pages

1. Create a new HTML template in the `templates` folder (e.g., `new_page.html`)
2. Add a new route in `app.py`:
```python
@app.route('/new-page')
def new_page():
    return render_template('new_page.html')
```
3. Create a link to your new page in the navigation menu (in `templates/base.html`)

## Git Workflow

1. Create a new branch for your changes:
```bash
git checkout -b feature/your-feature-name
```

2. Make your changes and commit them:
```bash
git add .
git commit -m "Description of your changes"
```

3. Push your branch to GitHub:
```bash
git push origin feature/your-feature-name
```

4. Create a Pull Request on GitHub to merge your changes into the main branch

## Project Structure

```
git_learner/
├── app.py              # Main application file
├── requirements.txt    # Python dependencies
├── static/            # Static files (CSS, JS, images)
│   └── style.css
└── templates/         # HTML templates
    ├── base.html      # Base template
    └── index.html     # Home page
``` 