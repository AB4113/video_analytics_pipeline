
✨ Features

• Real-Time Stream Processing: Ingests live RTSP camera feeds, local video files (.mp4, .avi), or webcam inputs.
• Object Detection & Tracking: Integrates modern object detectors with multi-object tracking algorithms to assign unique IDs across frames.
• Data Export: Generates annotated output video files alongside structured telemetry/metadata (JSON/CSV).
• Configurable Architecture: Easily swap models, adjust confidence thresholds, or define custom Region of Interest (ROI) zones.

🚀 Quick Start


Prerequisites

• Python 3.10+
• CUDA-compatible GPU (recommended for real-time inference)

Installation

1. Clone the repository:bash
git clone https://github.com
cd video_analytics_pipeline
Use code with caution.
2. Create and activate a virtual environment:bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Use code with caution.
3. Install dependencies:bash
pip install -r requirements.txt
Use code with caution.

💻 Usage

Run the pipeline on a local video file:
bash
python main.py --source data/sample.mp4 --weights models/yolo.pt --output output/result.mp4
Use code with caution.
Run the pipeline on a live RTSP stream:
bash
python main.py --source rtsp://username:password@ip_address:554/stream --output-display True
Use code with caution.

📁 Project Structure

text
video_analytics_pipeline/
├── data/               # Sample input videos and test clips
├── models/             # Pre-trained model weights
├── src/
│   ├── detector.py     # Object detection wrapper
│   ├── tracker.py      # Multi-object tracking logic
│   └── utils.py        # Helper functions for drawing and export
├── requirements.txt    # Python dependencies
├── main.py             # Pipeline entry point
└── README.md
Use code with caution.

🤝 Contributing

Contributions, bug reports, and feature requests are welcome!
1. Fork the repository.
2. Create your feature branch (git checkout -b feature/amazing-feature).
3. Commit your changes (git commit -m 'Add some amazing feature').
4. Push to the branch (git push origin feature/amazing-feature).
5. Open a Pull Request.

📄 License

This project is licensed under the MIT License. See the LICENSE file for details.
© 2026 Abenezer Beyene
