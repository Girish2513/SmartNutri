# 🥗 SmartNutri

**SmartNutri** is an intelligent nutrition assistant web application that helps users track their meals, monitor nutritional intake, set dietary preferences, and discover recipes. Built with Flask and integrated with the Nutritionix API, it provides a comprehensive solution for managing personal nutrition goals.

## 📌 Project Overview

SmartNutri is a web-based nutrition tracking application that enables users to:
- Search and identify foods with detailed nutritional information
- Log meals throughout the day (Breakfast, Lunch, Dinner)
- Track daily nutrition intake with visual charts
- Set personalized dietary preferences and goals
- Get recipe recommendations based on dietary needs
- Filter foods by nutritional tags (high/low proteins, carbohydrates, fats)


## ✨ Features

- 🔍 **Food Search & Identification** – Search foods using the Nutritionix API with detailed nutritional breakdown
- 📝 **Meal Logging** – Track what you eat for Breakfast, Lunch, and Dinner
- 📊 **Nutrition Tracking** – View daily nutritional intake with interactive charts powered by Chart.js
- 🎯 **Diet Preferences** – Set personalized calorie and macronutrient goals based on body information
- 🍳 **Recipe Suggestions** – Browse recipes filtered by dietary preferences (Vegan, Vegetarian, Non-Vegetarian)
- 🏷️ **Smart Food Tagging** – Foods are automatically tagged (High/Low Proteins, Carbohydrates, Fats)
- 📅 **Date-based Tracking** – View meal history by date
- 💾 **Local Food Database** – Add and manage custom foods in addition to the Nutritionix database
- 👤 **User Profiles** – Multi-user support with individual food logs and preferences

## 🛠 Tech Stack

### Backend
- **Flask** – Python web framework
- **Python 3** – Backend programming language
- **JSON** – Data storage for user profiles and food database

### Frontend
- **HTML5/CSS3** – Page structure and styling
- **JavaScript/jQuery** – Client-side interactivity
- **Chart.js** – Nutrition data visualization
- **DataTables** – Interactive tables for food search results
- **jQuery UI** – Date picker and sliders
- **Font Awesome** – Icons

### APIs & Libraries
- **Nutritionix API** – Comprehensive food nutrition database
- **Nutrition Label Plugin** – Display nutrition facts labels

## 📁 Project Structure

```
SmartNutri/
├── flask_server.py          # Main Flask application server
├── templates/               # HTML templates
│   ├── index.html          # Food search/identification page
│   ├── history.html        # Meal history page
│   ├── track.html          # Nutrition tracking page
│   ├── preference.html     # Diet preference settings
│   └── Recipes.html        # Recipe suggestions page
├── static/                 # Static assets
│   ├── bakeoff2.main.js    # Common JavaScript functions
│   ├── bakeoff2.index.js   # Food search functionality
│   ├── bakeoff2.history.js # Meal history functionality
│   ├── bakeoff2.track.js   # Nutrition tracking functionality
│   ├── bakeoff2.preference.js # Preference settings
│   ├── Recipe.js/Recipejs.js # Recipe functionality
│   ├── style.css           # Main stylesheet
│   └── chartjs/            # Chart.js library
├── food_data/              # Food database
│   ├── localFoods.json     # Custom food entries
│   └── nutrients.json      # Nutrient information
├── user_data/              # User profiles and data
│   ├── {user}_log.txt      # User meal logs
│   ├── {user}_pref.txt     # User preferences
│   └── {user}_dislike.txt  # User food dislikes
└── pictures/               # Application screenshots
```

## 📥 Installation Instructions

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

### 1. **Clone the Repository**
```bash
git clone https://github.com/Girish2513/SmartNutri.git
cd SmartNutri
```

### 2. **Install Python Dependencies**
```bash
pip install flask
```

### 3. **Configure Nutritionix API (Optional)**
The application uses the Nutritionix API for food data. The API credentials are included in the code, but you can get your own free API key at [Nutritionix Developer Portal](https://developer.nutritionix.com/).

To use your own API key, edit `static/bakeoff2.index.js`:
```javascript
var api_key = "your_api_key";
var app_id = "your_app_id";
```

### 4. **Start the Flask Server**
```bash
python flask_server.py
```

The server will start on `http://localhost:8000`

## ▶️ Usage

### Getting Started
1. Open your browser and navigate to: `http://localhost:8000`
2. The application supports multi-user functionality via URL parameters: `http://localhost:8000?user=username`

### Main Features

#### 🔍 Identify Food
- Search for foods using the search bar
- View detailed nutritional information including calories, carbohydrates, proteins, fats, vitamins, and minerals
- Add foods to your meal log by selecting the meal type (Breakfast, Lunch, Dinner) and date
- Add custom foods to the local database

#### 📝 Meal History
- View all logged meals organized by date and meal type
- See AI-generated nutritional tags for each food item
- Delete meals from your log
- Click on AI labels to see explanations

#### 📊 Track Nutrition
- View daily nutritional intake summaries
- Interactive charts showing calorie and macronutrient breakdown
- Compare actual intake against your dietary goals
- Track progress over time

#### 🎯 Diet Preference
- Enter body information (height, weight, age, gender)
- Calculate recommended daily calorie intake
- Set custom macronutrient distribution using sliders
- Define dietary rules and preferences
- Specify foods you dislike

#### 🍳 Recipes
- Browse recipes by dietary type:
  - Vegan recipes
  - Vegetarian recipes
  - Non-Vegetarian recipes
- Filter recipes based on your dietary preferences

## 🔌 API Endpoints

The Flask server provides the following RESTful endpoints:

- `GET /` - Main food identification page
- `GET /history.html` - Meal history page
- `GET /track.html` - Nutrition tracking page
- `GET /preference.html` - Diet preference page
- `GET /Recipes.html` - Recipe suggestions page
- `GET/POST /food-database` - Access/add foods to local database
- `GET/POST/DELETE /food-log?user={username}` - Manage user meal logs
- `GET/POST /food-pref?user={username}` - Manage user preferences
- `GET/POST /food-dislike?user={username}` - Manage user food dislikes
- `POST /food-tag-query` - Query foods by nutritional tags

## 🤝 Contributing

Contributions are welcome! If you'd like to improve SmartNutri:

1. Fork this repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the MIT License.
You are free to use, modify, and distribute this software.

## 💬 Contact

Repository maintained by Girish Saana
- GitHub: [@Girish2513](https://github.com/Girish2513)
- Email: girishsaana2513@gmail.com

## 📸 Screenshots

Check the `pictures/` directory for application screenshots showing:
- Food search interface
- Meal history view
- Nutrition tracking charts
- Diet preference settings
- Recipe recommendations
