# FloodML

Developed by Atanu Ghosh (June 2025)

![FloodML Logo](static/img/logo.png)

FloodML is an advanced web application that leverages **Machine Learning** to predict floods based on weather patterns and historical data. This tool aims to help communities prepare for and mitigate flood risks through accurate predictions and data visualization.

[![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![Flask Version](https://img.shields.io/badge/flask-1.1.2-green.svg)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.txt)

## Overview

### Quick Start 🚀

1. **Clone the Repository**
   ```bash
   git clone https://github.com/atanu0909/floodpredictionbyatanu.git
   cd floodpredictionbyatanu
   ```

2. **Set Up Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Run the Application**
   ```bash
   python app.py
   ```
   Visit `http://localhost:5000` in your web browser.

### Key Features 🌟
- Real-time flood prediction using machine learning
- Interactive heatmaps for risk visualization
- Satellite imagery integration
- Weather forecast integration
- User-friendly interface for predictions
- Historical data analysis and visualization

### Inspiration 💡
Floods, exacerbated by climate change, pose a growing threat worldwide. To address this, we created FloodML—an interactive web app for predicting and visualizing floods.

### Core Components

#### 1. Plots
- Flood Prediction Plot (Red dots for predicted flood locations)
- Precipitation Plot (Bubbles indicate precipitation volume)
- Damage Analysis Plot (Bubble size represents estimated monetary damage)

#### 2. Heatmaps
- Damage Analysis Heatmap (Colors indicate predicted monetary damage)
- Precipitation Heatmap (Dark red areas signify higher precipitation)
- Flood Prediction Heatmap (Darker red spots indicate likely flood locations)

#### 3. Satellite Images
- Displays precipitation volume over Indian cities
- Uses NASA's Global Precipitation Measurement Project data

#### 4. Predict Page
- Real-time weather forecast and flood prediction for any city
- Includes temperature, humidity, cloud cover, wind speed, and precipitation

### Development Process

#### The Dataset
- Scraped [floodlist.com](http://floodlist.com/tag/india) using Beautiful Soup 4
- Utilized Visual Crossing weather API for historic weather data
- Applied data augmentation techniques for model diversity

#### ML Model
- Built on the sci-kit learn library
- Explored various models; Random Forest Classifier achieved 98.71% accuracy
- Saved model using pickle

#### Data Visualization
- Integrated major Indian cities' data with weather factors
- Utilized Plotly chart studio for diverse map visualizations

#### Front-end and Hosting
- Developed with Flask framework
- Hosted on Heroku

### Challenges
- Limited data availability for floods in India
- Plotly integration complexities
- Git merge conflicts due to encoding and version disparities

### Achievements
- Created a robust dataset for accurate flood predictions
- Implemented a machine learning model with over 98% accuracy
- Successfully integrated data augmentation and visualization techniques

### Learnings
- Enhanced skills in web scraping, data mining, and Plotly
- Expanded proficiency in machine learning models

### Future Plans 🚀
- Expand coverage to cities worldwide
- Implement image classification for flood detection using satellite data
- Add real-time alerts and notification system
- Integrate with emergency response systems
- Develop mobile applications for wider accessibility

### Tech Stack 🛠️

#### Backend
- **Python 3.7+**: Core programming language
- **Flask**: Web framework for the application
- **Scikit-learn**: Machine learning models and predictions
- **Pandas & NumPy**: Data manipulation and numerical computations
- **Plotly**: Interactive data visualization
- **Beautiful Soup 4**: Web scraping for data collection

#### Frontend
- **HTML/CSS**: Structure and styling
- **JavaScript**: Interactive features
- **Bootstrap**: Responsive design framework
- **Ionicons**: Icon library
- **Owl Carousel**: Carousel/slider implementation

### Local Development 💻

#### Prerequisites
- Python 3.7 or higher
- Git
- pip (Python package installer)

#### Detailed Setup Steps
1. **Fork and Clone**
   ```bash
   git clone https://github.com/YOUR-USERNAME/floodpredictionbyatanu.git
   cd floodpredictionbyatanu
   ```

2. **Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: .\venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configuration**
   - Copy `.env.example` to `.env` (if exists)
   - Update environment variables as needed

5. **Run Development Server**
   ```bash
   python app.py
   ```
   The application will be available at `http://127.0.0.1:5000`

### Recent Updates 🆕
- Removed MySQL dependency for simpler local setup
- Updated package dependencies for better compatibility
- Enhanced documentation and setup instructions
- Fixed static asset loading issues
- Improved error handling in prediction module

### Contributing 🤝
1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make changes and commit (`git commit -am 'Add new feature'`)
4. Push to branch (`git push origin feature/improvement`)
5. Open a Pull Request

### Acknowledgments 👏
- [floodlist.com](http://floodlist.com/) for historical flood data
- Visual Crossing Weather API for weather data
- NASA's Global Precipitation Measurement Project
- Open-source community for various libraries and tools

### Contact 📫
- **Developer**: Atanu Ghosh
- **GitHub**: [@atanu0909](https://github.com/atanu0909)
- **Project Link**: [https://github.com/atanu0909/floodpredictionbyatanu](https://github.com/atanu0909/floodpredictionbyatanu)

### License 📄
This project is licensed under the MIT License - see the [LICENSE](LICENSE.txt) file for details.

---
Made with ❤️ by Atanu Ghosh
