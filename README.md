# 🧠 AI-Based Personality Prediction System

An intelligent system that analyzes social media text and predicts Big Five personality traits using NLP and Machine Learning.

## ✨ Features
- **Text Analysis**: Advanced NLP preprocessing with NLTK
- **Big Five Prediction**: OCEAN personality traits (Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism)
- **Interactive Web UI**: Modern, responsive interface
- **Real-time Visualization**: Radar charts and detailed breakdowns
- **Sample Texts**: Try different personality types
- **Instant Results**: Fast predictions with interpretations

## 🚀 Quick Start

### Option 1: Automated Setup
```bash
python setup.py
python app.py
```

### Option 2: Manual Setup
```bash
# Install dependencies
pip install -r requirements.txt

# Train the model
python model/train_model.py

# Run the application
python app.py
```

Then open http://localhost:5000 in your browser!

## 🏗️ Project Structure
```
├── model/
│   ├── personality_model.py    # ML model implementation
│   ├── preprocessor.py         # Text preprocessing
│   ├── train_model.py         # Training script
│   └── __init__.py
├── static/
│   ├── style.css              # Frontend styling
│   └── script.js              # Frontend logic
├── templates/
│   └── index.html             # Main web interface
├── saved_models/              # Trained models (created after training)
├── app.py                     # Flask web application
├── requirements.txt           # Python dependencies
├── setup.py                   # Automated setup script
└── README.md
```

## 🔧 Tech Stack
- **Backend**: Flask + scikit-learn
- **Frontend**: HTML/CSS/JavaScript + Chart.js
- **NLP**: NLTK + TF-IDF Vectorization
- **Model**: Multi-output RandomForest Regression
- **Visualization**: Chart.js radar charts

## 🎯 How It Works

1. **Text Input**: User enters text (social media posts, thoughts, etc.)
2. **Preprocessing**: 
   - Clean text (remove URLs, punctuation)
   - Tokenization and lemmatization
   - Remove stopwords
   - TF-IDF vectorization
3. **Prediction**: Multi-output regression model predicts 5 traits
4. **Visualization**: Results displayed as percentages with radar chart
5. **Interpretation**: Human-readable personality analysis

## 📊 Big Five Personality Traits (OCEAN)

- **Openness**: Creativity, curiosity, openness to new experiences
- **Conscientiousness**: Organization, discipline, goal-oriented behavior  
- **Extraversion**: Sociability, energy, preference for interaction
- **Agreeableness**: Cooperation, trust, concern for others
- **Neuroticism**: Emotional instability, negative emotions

## 🧪 Sample Usage

Try these sample texts to see different personality profiles:

**Creative Person**: "I love exploring new ideas and creative projects..."
**Organized Person**: "I always plan my day carefully and stick to my schedule..."
**Social Person**: "I absolutely love meeting new people and being around others..."

## 🔍 API Endpoints

- `GET /` - Main web interface
- `POST /predict` - Personality prediction API
- `GET /health` - Health check

## 🚀 Deployment Options

### Local Development
```bash
python app.py
# Access at http://localhost:5000
```

### Production Deployment
The app is ready for deployment on:
- **Render**: Connect GitHub repo, set build command to `python setup.py`
- **Railway**: Deploy with automatic builds
- **Heroku**: Add Procfile: `web: python app.py`
- **HuggingFace Spaces**: Upload as Gradio/Streamlit alternative

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📝 License

This project is open source and available under the MIT License.

## 🎉 Acknowledgments

- Built with Flask, scikit-learn, and NLTK
- Uses Big Five personality model
- Inspired by modern personality psychology research
