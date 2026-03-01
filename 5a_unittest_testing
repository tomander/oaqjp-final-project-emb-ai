from EmotionDetection.emotion_detection import emotion_detector

import unittest

class TestDetector(unittest.TestCase): 

    def testJoy(self): 
        emotions = emotion_detector("I am glad this happened")
        dominant = max(emotions, key=emotions.get)
        self.assertEqual(dominant, "joy")

    def testAnger(self): 
        emotions = emotion_detector("I am really mad about this")
        dominant = max(emotions, key=emotions.get)
        self.assertEqual(dominant, "anger")

    def testDisgust(self): 
        emotions = emotion_detector("I feel disgusted just hearing about this")
        dominant = max(emotions, key=emotions.get)
        self.assertEqual(dominant, "disgust")

    def testSadness(self): 
        emotions = emotion_detector("I am so sad about this")
        dominant = max(emotions, key=emotions.get)
        self.assertEqual(dominant, "sadness")

    def testFear(self): 
        emotions = emotion_detector("I am really afraid that this will happen")
        dominant = max(emotions, key=emotions.get)
        self.assertEqual(dominant, "fear")

unittest.main()