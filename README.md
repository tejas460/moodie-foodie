# MoodieFoodie  
*Food for Every Mood*  

**MoodieFoodie** is a revolutionary web application that suggests food based on your mood using machine learning and delivers it to your doorstep.  

---

## Why MoodieFoodie?  

The question might arise: **"How is this different from other food delivery apps?"**  
Let us explain why MoodieFoodie stands out:  

### 1. Optimized Restaurant Suggestions:  
Unlike traditional apps that filter restaurants using one criterion at a time (cost, rating, or distance), MoodieFoodie recommends restaurants that balance all three parameters:  
- **Cost**  
- **User Ratings**  
- **Distance**  

This saves you time and ensures you get the best value without compromises.

### 2. Mood-Based Food Suggestions:  
Struggling with the eternal question: **"What to eat?"** MoodieFoodie has got you covered!  
- Based on your current mood—be it happy, sad, angry, or even unwell—the app suggests the perfect food to match your feelings.  
- Powered by machine learning, it learns from past users' mood-food choices to give you personalized recommendations.

### 3. Unique Features for Every Scenario:  
- See the most-ordered items for a specific time of day.  
- Get food delivered in the shortest possible time when you're in a rush.  
- Discover trending and top-searched food items.  

### 4. Support for Small Businesses:  
- Order items like tea, juices, or even homemade chocolates, thanks to our "Wanna Sell on MoodieFoodie" feature.  
- We enable small-scale sellers (like tea shops or home-based chocolatiers) to expand their reach and sell online.

---

## Working and Implementation  

### Key Features  

#### 1. Restaurant Recommendations:  
- **User Ratings:**  
  Restaurants are rated by users (out of 5). The ratings are dynamically updated using the mathematical average of the previous and new ratings.  
- **Cost for Two:**  
  Stored as static data in the database.  
- **Distance Calculation:**  
  The app uses stored restaurant geocodes and Google Maps API to calculate the user's distance from a restaurant.

The data is processed using **Logistic Regression**, a simple yet effective machine learning model. When a user selects a restaurant, their preferences are recorded to improve recommendation accuracy.

#### 2. Mood-Based Food Suggestions:  
- The app uses past user data (moods and food orders) to train a machine learning model.  
- Over time, the algorithm becomes more accurate in pairing moods with suitable food choices.

#### 3. Small Business Integration:  
- A form is provided for small-scale sellers to submit their details and join the platform.  
- Their offerings are listed alongside mainstream restaurants.

---

## Installation Requirements  

### Frameworks and Libraries  
- **Framework:** Django, Version: 1.11.8  
- **Language:** Python, Version: 3.6.3  

### Required Packages  
- Bootstrap 3  
- numpy  
- sklearn  
- bcrypt  
- django[argon]  

### Installation Command  
```bash
pip install package-name
