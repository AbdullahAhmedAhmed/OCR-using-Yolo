# OCR-using-Yolo
In this project i will use YOLO object detection to train a model to detect Egyptian license plates from images and videos. Egyptian license plates have a unique format that makes them identifiable, with the car's character  written in Arabic  beside a series of numbers on the bottom of the car. By training YOLO on a dataset(1200 simple for training ,301 for test 499 for validation) of labeled Egyptian license plate images, I will build a model that can accurately locate license plates within complex scenes.

Once the YOLO model is trained, I will use it to detect license plates from new, unlabeled images and videos. YOLO will output the coordinates of any detected license plates regions. I will then programmatically crop out just those regions from the original images/frames. This will give me sub-images containing only the license plate contents, with the background removed.

At that point, I plan to use EasyOCR to recognize the text within each license plate crop. EasyOCR is an optical character recognition tool that is well-suited for Arabic script. By feeding it the license plate crops, it should be able to read both the Arabic name on top and the numbers on the bottom. This will give me the full text contents of each detected license plate.



I trained my model with data that you will find in this link :https://drive.google.com/drive/folders/11PRO0HoZwlqFlxkJbAy0fsL-WXW9xhME?usp=sharing
Note: I used CVAT https://www.cvat.ai/ to label the data to be fit in my model in CVAT you will see different format for exported labeled data choose txt option if you will use yolo or any ssd model
