#  Banking System with Facial Recognition

A secure and user-friendly digital banking system that uses **facial recognition** instead of traditional PINs for user authentication during transactions. Built as part of my final year project.

##  Features

-  **Face Detection & Recognition**: Real-time face authentication using stored face embeddings.
-  **User Registration**: Register new users with their facial data.
-  **Login & Authentication**: Authenticate users with facial recognition for secure access.
-  **Transaction Processing**: Perform basic banking transactions post-authentication.
-  **GUI with Tkinter**: Intuitive interface for easy interaction.
-  **Data Handling**: Facial data stored securely using Python's `pickle`.

##  Tech Stack

- **Language**: Python
- **Libraries**: OpenCV, dlib, face_recognition, Tkinter
- **Storage**: Pickle for storing face embeddings

##  How It Works

1. **User Registration**  
   - User provides name and facial image via webcam  
   - System extracts facial embeddings and stores them with the user’s name

2. **Login**  
   - Captures a live image via webcam  
   - Compares live facial embeddings with stored ones  
   - Authenticates the user if a match is found

3. **Transaction**  
   - Once logged in, the user can perform a dummy transaction (simulation for demo)

##  Limitations

-  No liveness detection (vulnerable to photo attacks)
-  No session logout or time-based session handling
-  Face embeddings stored in local files, not a secure database

##  Future Improvements

- Add **liveness detection** for improved security  
- Integrate **secure backend storage** (e.g., database with encryption)  
- Implement **multi-user session management**  
- Add **transaction history logs**

##  Setup Instructions

1. Clone the repository  
   ```bash
   git clone https://github.com/yourusername/banking-face-recognition.git
   cd banking-face-recognition
2. From requirements file you can install everything at once by running following command
    ```bash
    pip install -r requirements.txt