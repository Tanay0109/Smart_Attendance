Smart_Attendance
• Architected and integrated a face recognition model into a Flask-based backend server, enabling automated attendance tracking for 300+ students and efficient data storage using Raspberry Pi.
• Designed and launched a user-friendly web portal for seamless management of attendance records and user data, enhancing administrative efficiency.
• Deployed the solution on Raspberry Pi to ensure portability and cost-effectiveness, making it suitable for classroom and training environments.
• Improved recognition accuracy under varying lighting conditions using jitter-based data augmentation during face encoding.
• Developed core backend logic in flask_app.py to handle real-time recognition, logging, and course-specific attendance tracking.
• Implemented helper utilities in utils.py for time management, user handling, and log formatting.
• Created a clean frontend interface using HTML, CSS, and JavaScript, stored in the assets/ directory.

Setup Instructions
• Clone the repository:

bash
Copy
Edit
git clone https://github.com/Tanay0109/Smart_Attendance.git
cd Smart_Attendance
• (Optional) Create and activate a virtual environment:

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
• Install required packages:

bash
Copy
Edit
pip install flask face_recognition opencv-python numpy
• Run the application:

bash
Copy
Edit
python flask_app.py
• Access the web interface at:

arduino
Copy
Edit
http://localhost:5000/
Key Files
• flask_app.py: Main application logic (routes, attendance tracking, data handling)
• model.py: Handles facial encoding and recognition logic
• utils.py: Utility functions for file handling and timestamps
• assets/: Frontend files including HTML, CSS, and JS
• app.py: Basic Flask app runner (used during testing)

Applications
• Built to automate and streamline attendance tracking in academic settings
• Minimizes manual errors and proxy attendance
• Can be adapted for use in training centers, office check-ins, and small-scale events

