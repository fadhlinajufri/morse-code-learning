## Requirements
1. Functional requirements
FR1: The system shall capture live video from a standard webcam.
FR2: The system shall detect facial landmarks around the eyes and calculate the EAR in every frame.
FR3: The system shall classify a blink shorter than the duration threshold as a dot and a blink equal to or longer than it as a dash.
FR4: The system shall present a lesson showing 1–3 randomly selected letters or numbers together with their Morse code patterns.
FR5: The system shall give an exercise that asks the user to reproduce a given character through blinks.
FR6: The system shall show immediate feedback (correct or incorrect) after each exercise attempt.
FR7: The system shall record each user’s exercise results and show their score at the end of a session.

2. Non-functional requirements
NFR1 (Performance): The system shall process webcam frames and show the detected dot or dash within 0.5 seconds of the blink ending, at a minimum of 15 frames per second.
NFR2 (Usability): A new user shall be able to complete calibration and start the first lesson within 3 minutes, without help from a developer.
NFR3 (Reliability): The system shall achieve at least 90% blink classification accuracy (dot vs dash) under normal indoor lighting.
NFR4 (Compatibility): The system shall run on a laptop with a built-in 720p webcam and no extra hardware.

