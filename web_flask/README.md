mkuu## Web Framework
A web framework is a software framework that provides a structured way to build and develop web applications. 
- It includes pre-built components, libraries, and tools that facilitate the creation of web applications by providing common functionality, such as handling HTTP requests, managing routes, and handling database interactions.

## Flask
Flask is a micro-web framework for Python that is lightweight and easy to use. 
- It provides the basic tools and libraries needed to build a web application, but it doesn't come with many pre-built features, allowing developers to choose and add components as needed.

To build a web framework with Flask, you would typically follow these steps:

1. **Install Flask:** First, you need to install Flask. You can do this using pip, Python's package manager, with the following command:
```
pip install Flask
```

2. **Create a Flask Application:** Create a Python file (e.g., app.py) and import the Flask module:
```
from flask import Flask

app = Flask(__name__)
```

3. **Define Routes:** In Flask, routes are the URL paths that your application will respond to. You define routes using the @app.route decorator. For example:
```
@app.route('/')
def index():
    return 'Hello, World!'
```

- In this example, when a user navigates to the root URL (/), the function index will be executed, and it will return the string 'Hello, World!'.

4. **Run the Application:** At the end of your script, add the following code to run the Flask application:
```
if __name__ == '__main__':
    app.run(debug=True)
```
- This starts the Flask development server.

5. **Start the Application:** In your terminal, navigate to the directory containing app.py and run it using:
```
python app.py
```
