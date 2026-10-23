# Specialized Technology
Computer Vision

## 1. Eye Aspect Ratio (EAR) Method
This project uses the Eye Aspect Ratio (EAR) method to detect eye blinks through a standard webcam. It measures changes in the distance between facial landmarks around the eyes to identify whether the eyes are open or closed. Short and long intentional blinks can then represent Morse code dots and dashes.

## 2. Benefits and Limitations
The EAR method is low-cost, contactless and suitable for real-time feedback. Furthermore, it does not require training data or model training. Calibration can also help adjust blink detection for different users.
However, lighting conditions, camera angles and individual differences may affect detection accuracy. In addition, natural blinks may be mistaken for intentional inputs. Therefore, a minimum-duration filter is needed.

## 3. Alternative Technologies
Convolutional Neural Network (CNN) can classify eye images as open or closed. But, it requires labelled data, more computing power and additional development time

Another option is to use Electrooculography (EOG) sensors or dedicated eye trackers. Although these technologies can provide precise eye movement measurements, they are generally more expensive, and EOG sensors require physical contact.

## 4. Technology Selection
The computer vision using EAR method is selected because it is affordable, contactless and suitable for real-time eye blink detection without requiring model training
