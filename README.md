# 🏋️ AI Gym Coach

A real-time AI-powered fitness coach built with **Streamlit**. It uses your webcam to track your body pose, analyze your exercise form, count reps, and give you instant feedback, with AI-generated coaching and voice guidance.

<!-- Add a screenshot or demo GIF here -->
<!-- ![AI Gym Coach Demo](./static/demo.png) -->

🔗 **Live Demo:** [https://musical-syrniki-77ab75.netlify.app](https://musical-syrniki-77ab75.netlify.app/)

---

## ✨ Features

- 🎥 **Real-time pose detection** using your webcam (MediaPipe)
- 🔢 **Automatic rep counting** for supported exercises
- ✅ **Form analysis** with instant corrective feedback
- 🤖 **AI coaching** powered by the Groq LLM API
- 🔊 **Voice feedback** using text-to-speech (gTTS)
- 📊 **Workout data tracking** with Pandas
- 📚 **Tutorial info** to help you learn each exercise correctly
- 🖥️ Clean multi-page Streamlit interface

---

## 🛠️ Tech Stack

| Category          | Technologies                      |
| ----------------- | --------------------------------- |
| Framework / UI    | Streamlit, streamlit-webrtc       |
| Computer Vision   | MediaPipe, OpenCV                 |
| AI / LLM          | Groq API                          |
| Text-to-Speech    | gTTS                              |
| Data              | Pandas                            |
| Config            | python-dotenv                     |
| Language          | Python                            |

---

## 📁 Project Structure

```
ai-gym-coach-streamlit/
├── core/             # Core logic and shared utilities
├── detectors/        # Exercise detection and pose analysis
├── ml_models/        # Machine learning models
├── pages/            # Streamlit multi-page app screens
├── services/         # External services (AI coach, voice, etc.)
├── static/           # Images and static assets
├── tutorial-info/    # Exercise tutorials and guides
├── main.py           # App entry point
├── packages.txt      # System-level dependencies (for deployment)
├── requirements.txt  # Python dependencies
└── .gitignore
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10 or 3.11 (recommended for MediaPipe compatibility)
- A working webcam
- A free [Groq API key](https://console.groq.com/)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/KaranKumar7646/ai-gym-coach-streamlit.git
cd ai-gym-coach-streamlit

# 2. (Recommended) Create a virtual environment
python -m venv venv

# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate

# 3. Install dependencies
pip install -r requirements.txt
```

### Set up environment variables

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key_here
```

> ⚠️ Never commit your `.env` file or API keys to GitHub.

### Run the app

```bash
streamlit run main.py
```

Open `http://localhost:8501` in your browser and allow camera access when prompted.

---

## 🧑‍🏫 How to Use

1. Open the app and allow webcam access.
2. Choose an exercise from the menu.
3. Stand where your full body is visible to the camera.
4. Start exercising. The app counts your reps and checks your form.
5. Listen to or read the AI coach's feedback to improve.

---

## ☁️ Deployment

This app can be deployed on [Streamlit Community Cloud](https://streamlit.io/cloud):

1. Push the repo to GitHub.
2. Create a new app on Streamlit Cloud and select `main.py` as the entry file.
3. Add `GROQ_API_KEY` under **Settings → Secrets**.
4. Deploy. System packages listed in `packages.txt` are installed automatically.

---

## 🔮 Future Improvements

- Support for more exercises
- Workout history and progress charts
- Personalized workout plans
- Mobile-friendly experience

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📬 Contact

**Karan Kumar**

- GitHub: [@KaranKumar7646](https://github.com/KaranKumar7646)
- LinkedIn: [Karan Kumar](https://www.linkedin.com/in/karan-kumar-687854282/)
- LeetCode: [KaranKumar7646](https://leetcode.com/KaranKumar7646)
- Email: itskaran7646@gmail.com

---

⭐ If you found this project useful, please give it a star!
