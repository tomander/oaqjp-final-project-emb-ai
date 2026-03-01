"""Web app"""
from flask import Flask, render_template, request
from EmotionDetection.emotion_detection import emotion_detector

app = Flask("Emotiuonal Detector")

@app.route("/emotionDetector")
def sent_analyzer():
    """Do detection"""
    text_to_analyze = request.args.get('textToAnalyze')
    response = emotion_detector(text_to_analyze)
    return response

@app.route("/")
def render_index_page():
    """Show main page"""
    return render_template('index.html')


if __name__ == "__main__":
    app.run(port=5000)
