# Specialized Technology
Computer Vision

## Benefits and Limitations
The Eye Aspect Ratio (EAR) method is low-cost, contactless and suitable for real-time feedback using a standard webcam. Furthermore, it does not require training data or model training while calibration helps adjust blink detection for different users
However, lighting, camera angles and individual differences may affect detection accuracy. In addition, natural blinks may be mistaken for intentional inputs. Therefore, a minimum-duration filter is needed. For privacy, webcam video should be processed locally and not stored (NFR4)

## Alternative
A CNN can classify eye images but requires labelled data, greater computing power and more development time. EOG sensors and eye trackers may provide more precise measurements. However, they are generally more expensive and may require physical contact.

Therefore, the EAR method is chosen because it is affordable, contactless and does not require model training