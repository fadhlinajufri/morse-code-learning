# Specialized Technology
## Computer Vision
Computer vision is a field of artificial intelligence that allows computers to obtain useful information from images and videos. Computer vision tools offer the possibility to track manual and non-manual movements such as eye blinks in a non-invasive and scalable way (Susman, M., Blasco, C. M., & Bulla, J., 2026). It captures a frame and finds the object of interest then locates key points on it, calculating a measurement from those points and makes a decision using a rule or trained model. In this project, the object of interest is the user’s face, the key points are the landmarks around the eyes, the measurement is the Eye Aspect Ratio (EAR) and the decision is whether a blink is a dot or a dash.

## Eye Aspect Ratio (EAR) Method
It measures changes in the distance between facial landmarks around the eyes to identify whether the eyes are open or closed

 P1 : Left corner 
 P2 : Upper lid, left 
 P3 : Upper lid, right 
 P4 : Right corner 
 P5 : Lower lid, right 
 P6 : Lower lid, left 

When the eye is open the vertical distances are large, so the EAR is high. When the eye closes they are close to zero, so the EAR drops (Rosebrock, 2017). Eyes differ between people, so the threshold is set during calibration. Blink duration is the time the EAR stays below the threshold: a short blink is a dot and a long blink is a dash

## Worked example
After calibration, the EAR threshold is 0.20 and the dot/dash boundary is 0.4 s. To blink the letter A (· –):

1. The user keeps the EAR below 0.20 for 0.2 s. This is shorter than 0.4 s, so it is a dot
2. The user then keeps the EAR below 0.20 for 0.6 s. This is longer than 0.4 s, so it is a dash
3. The system reads · – matches it to A and shows "Correct"

## Benefits and Limitations
The EAR method is low-cost, contactless and suitable for real-time feedback. Furthermore, it does not require training data or model training. Calibration can also help adjust blink detection for different users.
However, lighting conditions, camera angles and individual differences may affect detection accuracy. In addition, natural blinks may be mistaken for intentional inputs. Therefore, a minimum-duration filter is needed.

## Alternative Technologies
Convolutional Neural Network (CNN) can classify eye images as open or closed. But, it requires labelled data, more computing power and additional development time

Another option is to use Electrooculography (EOG) sensors or dedicated eye trackers. Although these technologies can provide precise eye movement measurements, they are generally more expensive, and EOG sensors require physical contact.

## Sources
1. Kannan, A., Vinoj, A., Pathirikattil, A., Prasad, D. V., & Moozhippurath, B. (April, 2026). An AI-Based Hands-Free Communication System Using Eye Blinks and Morse Code with YOLOv8 and LSTM Prediction. International Conference on AI-Driven Solutions for Sustainable Smart Cities: Challenges and Opportunities (ADSSSC), (pp. 1-6). doi:10.1109/ADSSSC67751.2026.11582006
2. Pavithraa, & Kujani, T. (May, 2026). Eye Blink–based Morse Code Translation for Assistive Communication using a MobileNetV2–LSTM Framework. Eye Blink–based Morse Code Translation for Assistive Communication using a MobileNetV2–LSTM Framework. 2026 7th International Conference on Intelligent Communication Technologies and Virtual Mobile Networks (ICICV), pp. 725-730. doi:10.1109/ICICV68925.2026.11554634
3. Rosebrock, A. (2017). Eye blink detection with OpenCV, Python, and dlib. Retrieved from https://pyimagesearch.com/2017/04/24/eye-blink-detection-opencv-python-dlib/
4. Sushmitha, S., Prasad, H. B., & Sapna, V. M. (2025). Multi-layer Secure Authentication using Morse Code and Eye Blink Detection. 2025 9th International Symposium on Innovative Approaches in Smart Technologies (ISAS), pp.1-8. doi:10.1109/ISAS66241.2025.11101975
5. Susman, M., Blasco, C. M., & Bulla, J. (May, 2026). Comparing Computer Vision Instruments for Eye Blink Analysis. Proceedings of the LREC 2026 12th Workshop on the Representation and Processing of Sign Languages: Language in Motion, (pp. 459-467). Retrieved from https://aclanthology.org/2026.signlang-1.47.pdf
6. Umale, G., Kulkarni, P., Tyagi, A., Korgaonkar, A., & Tikale, D. (2026). Intelligent Morse Code Translation Framework and Authentication.



