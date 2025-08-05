# Bengaluru_House_price_prediction

A web application that predicts home prices in Bangalore using machine learning.

## Tech Stack

HTML, CSS, JavaScript, Python, Flask, scikit-learn, pickle, JSON, VS Code

## Features

- Predicts home prices based on area, BHK, bath, and location
- Interactive web interface
- Real-time predictions using a trained ML model

## Project Structure

```
BHP/
├── client/
│   ├── app.html
│   ├── app.js
│   ├── app.css
├── server/
│   ├── server.py
│   ├── util.py
│   └── artifacts/
│       ├── columns.json
│       └── banglore_home_prices_model.pickle
```

## Setup Instructions

1. **Clone the repository**
   ```
   git clone https://github.com/yourusername/bangalore-home-price-prediction.git
   cd bangalore-home-price-prediction/BHP
   ```

2. **Install Python dependencies**
   ```
   pip install flask scikit-learn numpy
   ```

3. **Run the Flask server**
   ```
   cd server
   python server.py
   ```
   The server will start at `http://127.0.0.1:5000/`.

4. **Serve the frontend**
   - Open a new terminal and navigate to the `client` directory:
     ```
     cd ../client
     python -m http.server 8000
     ```
   - Open [http://localhost:8000/app.html](http://localhost:8000/app.html) in your browser.

## Usage

1. Enter the area (in square feet), select BHK, bath, and location.
2. Click "Estimate Price" to get the predicted price.

## License

This project is licensed under
