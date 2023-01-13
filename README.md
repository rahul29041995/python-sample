# python-sample

# Create main.py

from flask import Flask

app = Flask(__name__)

@app.route("/")
def index():
    return "Congratulations, it's a web app!"
    
# Create requirements.txt
Flask==2.1.2

# Create app.yaml
runtime: python310

####### Test Locally #######
python -m venv venv
venv/bin/activate
python3 -m pip install -r requirements.txt

## Add the below script to main.py 

if __name__ == "__main__":
    app.run(host="127.0.0.1", port=8080, debug=True)

Execute : python main.py

O/P 

 * Serving Flask app "main" (lazy loading)
 * Environment: production
   WARNING: This is a development server.
   Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Running on http://127.0.0.1:8080/ (Press CTRL+C to quit)
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 315-059-987

