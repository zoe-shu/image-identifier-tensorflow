#Image Identifier with TensorFlow.js
```sh
$ yarn install
$ yarn watch
```

#Usage
1. allow browser to use web camera
2. show below images to the web camera
3. the identified result shown on right side

![image](https://github.com/zoe-shu/image-identifier-tensorflow/blob/master/dist/img/card1_front.jpg)
![image](https://github.com/zoe-shu/image-identifier-tensorflow/blob/master/dist/img/card2_front.jpg)
![image](https://github.com/zoe-shu/image-identifier-tensorflow/blob/master/dist/img/card3_front.jpg)
<img src="https://github.com/zoe-shu/image-identifier-tensorflow/blob/master/dist/img/postcard_back.png" width="150" />

- This program is based on "TensorFlow.js Example: Transfer Learning to play Pacman via the Webcam"
- node.js v8.12 required


# Update learning model file
index.js Line:184
-model.json path

# identified result response to another website/client/server
ui.js Line:22
-kiosk's socket.io path

# Re-train Model Instruction:
Re-train model and download:
1. comment index.js Line225 "await clickLoad();"
2. uncomment index.js Line206 "dlModel();"
3. frontend click the img div to take sample, then click "Train", then click "Play" to download trained model.JSON
4. uncomment index.js Line225 "await clickLoad();"
5. comment index.js Line206 "dlModel();"

This example shows you how to predict poses from a webcam using transfer
learning.
