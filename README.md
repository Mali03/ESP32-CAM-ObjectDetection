# ESP32-Cam Edge Impulse Object Detection

This project uses an ESP32-CAM (AI Thinker) module to run an Edge Impulse–trained AI object detection model and stream the results live through a web browser.

Camera frames are processed directly on the ESP32, objects are detected using the AI model, and bounding boxes with labels and confidence scores are drawn on the live video stream.

<p float="left">
  <img src="/Result Example 1.png" width="350" />
  <img src="/Result Example 2.png" width="350" />
</p>

## Getting Ready
To code ESP32 Cam, you need to do:
1) Open Arduino IDE -> File -> Preferences
2) Add `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json` to **Additional boards manager URLs**

## Collecting Data to Train AI Model 
1) Open Arduino IDE -> Library Manager
2) Install `EloquentEsp32Cam` library
3) Go File -> Examples -> EloquentEsp32Cam -> Collect_Images_for_EdgeImpulse
4) Install the code to ESP32 Cam (To program look at [Programming ESP32 Cam](#programming-esp32-cam))

## Programming ESP32 Cam
The ESP32-CAM does not include an integrated USB-to-serial programmer so an external FTDI (USB-to-TTL) programmer is used for uploading code.
<p float="left">
  <img src="/FTDI Programmer Pinout.png" width="500" />
</p>
