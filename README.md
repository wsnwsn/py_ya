from flask import Flask

app = Flask(__name__)


@app.route('/')
@app.route('/index')
def index():
    return "<h1>Привет, Яндекс! Я - Соня<h1>"


if __name__ == '__main__':
    app.run(port=8080, host='127.0.0.1')