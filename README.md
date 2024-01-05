# -Web-Application
Full-Stack Web Application with Flask and React:
# Flask (backend) - app.py
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')

if __name__ == '__main__':
    app.run(debug=True)

# React (frontend) - App.js
import React from 'react';

function App() {
    return (
        <div>
            <h1>Hello, React!</h1>
        </div>
    );
}

export default App;
