# Ethio-defense-deepfake-detection-
# README.md for DeepFake Detection Project

# Web-Based and CLI DeepFake Detection System
**Author:** Pvt Soldier Binyam E.
**GitHub:** [https://github.com/Binyam-Endale](https://github.com/Binyam-Endale)
**For:** Ethiopian Military Cyber Defense Directorate

---

## Project Summary
This project provides a beginner-friendly Python-based DeepFake Detection System with both CLI and Web UI interfaces. It detects manipulated media (images, video, audio) and displays results in English and Amharic (ነው / አይደለም). The system is designed to run locally on localhost for security purposes.

## Features
- **CLI Tool:** Evaluate media quickly from the command line.
- **Web UI:** Upload media and view results in a user-friendly interface.
- **Detection Metrics:** Accuracy, false positives, and false negatives.
- **Security:** Media processed locally; no data is uploaded online.

## Project Structure
```
deepfake_detection_project/
│
├─ cli_app.py          # CLI detection script
├─ web_app.py          # Flask Web UI (localhost)
├─ models/             # Pre-trained detection models
├─ static/             # Images, CSS for Web UI
├─ templates/          # HTML templates for Web UI
├─ README.md           # Project documentation
└─ requirements.txt    # Required Python packages
```

## Setup Instructions
1. Clone the repository:
```bash
git clone https://github.com/Binyam-Endale/deepfake_detection_project.git
```
2. Navigate into the project folder:
```bash
cd deepfake_detection_project
```
3. Install required Python packages:
```bash
pip install -r requirements.txt
```

## Usage
### CLI
```bash
python cli_app.py --input <path_to_media>
```
- Outputs results in English + Amharic.
- Shows detection metrics.

### Web UI
```bash
python web_app.py
```
- Open a browser and go to `http://localhost:5000`
- Upload media and view detection results.
- Footer includes author contact info.

## Evaluation Metrics
- Accuracy: Correct detection rate
- False positives / False negatives
- Metrics displayed after evaluation

## Future Expansion
- Real-time detection integration
- Integration with other military monitoring systems
- Optional cloud deployment for centralized secure analysis

## References / Tools
- Python libraries: `opencv-python`, `torch`, `flask`, `deepface`
- Reference GitHub projects for deepfake detection
- Research papers on deepfake detection techniques

## Contact
- Facebook: [Your Facebook link]
- GitHub: [https://github.com/Binyam-Endale](https://github.com/Binyam-Endale)
- Email: [Your email]
- Phone: [Your phone number]
