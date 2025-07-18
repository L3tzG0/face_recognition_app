# face_recognition_app

👁️‍🗨️ Face Recognition System
A real-time computer vision project that performs face recognition, gender detection, and age prediction, complete with attendance logging using OpenCV, Keras, and FaceNet.

🚀 Features
- Real-time webcam-based face detection and recognition
- Predicts gender and approximate age using pre-trained CNN models
- Embeds known faces and stores them in a .pkl database
- Attendance logging saved in timestamped Excel sheet
- Clean modular design: separate scripts for capture, embedding, and execution

🧠 Tech Stack
- Python, OpenCV, Mediapipe, Keras, TensorFlow, FaceNet
- Excel (via pandas) for logging
- Haar Cascade for face detection fallback

🗂️ Project Structure

 	project-root/
 	├── camera.py         # Capture new face images
  	├── capture.py        # Generate embeddings and store them
 	├── main.py           # Real-time recognition and demographic predictions
	├── embeddings/
 	│   └── data.pkl      # Face embeddings database
	├── model/
 	│   ├── gender_detection20.h5
	│   └── age_model_efficientnet.h5
	├── pics/             # Captured training images
	├── attendance_*.xlsx # Output logs
	└── requirements.txt

🧪 Getting Started
Clone the repo and install dependencies:

	bash
	pip install -r requirements.txt
 
Run camera.py to collect face images:

 	python camera.py
Generate embeddings:

 	python capture.py
Run the main system:
	
 	python main.py

📝 Notes
- Ensure model files and data paths are correctly placed
- Uses webcam (can be swapped for pre-recorded footage)
- Requires at least one identity with embeddings to function properly
- Project was made using python 3.10.11

👥 Credits
This project was developed collaboratively by a team of four students.
- Dhruv – Led the integration of multiple models into a single cohesive application. Created the camera.py, capture.py, and main.py scripts. Developed and implemented the gender detection pipeline.
- Other Contributors – Worked together on model preparation, testing, and refining the application.

	_The final codebase includes contributions and refinements from all team members._
