# Recommender System Demo using Matrix Factorization (NMF)
This notebook demonstrates a simple video game recommender system built with the Surprise library. It uses matrix factorization (NMF) to predict user–game ratings and recommend top games.

## Features
- **User-based Recommendations**: Get personalized game recommendations for any user
- **Synthetic Ratings**: Simulates user ratings derived from real-world sales data
- **Model Evaluation**: Performance metrics (Precision@5, Recall@5, RMSE)
- **Unseen Game Prediction**: Predicts ratings for games a user hasn't rated yet

## Dataset
The system uses one CSV file (Best Selling Video Games dataset):
- `best_selling_video_games.csv`: Contains game information (Rank, Title, Platform, Developer, Publisher, ReleaseYear, Sales, Series)

## Requirements
- Python 3.7+
- Dependencies listed in `requirements.txt`

## Installation & Setup

### 1. Clone the Repository
```bash
git clone <your-repository-url>
```

### 2. Create Virtual Environment (Recommended)
```bash
# Create virtual environment
python -m venv game_rec_env

# Activate virtual environment
# On macOS/Linux:
source game_rec_env/bin/activate

# On Windows:
game_rec_env\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

## Usage

### Running the Jupyter Notebook
1. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

2. **Open the notebook**: Navigate to and open `prasad.ipynb`

3. **Run all cells**: Execute all cells in order by selecting "Cell" → "Run All" or run each cell individually with `Shift+Enter`

## Expected Output
When you run the notebook, you should see:

1. **Model Training Progress**: surprise.model_selection
2. **Evaluation Metrics**:
   - Precision@5: ~0.60
   - Recall@5: ~0.45
   - RMSE: ~0.95
3. **Sample Recommendations**: Personalized game recommendations for users 1, 50, 100
4. **Predict ratings for unseen games for specific users**: users 1, 50, and 100

## File Structure
```
videogame-recommender/
├── prasad.ipynb                      # Main Jupyter notebook
├── best_selling_video_games.csv      # Game dataset
├── requirements.txt                  # Dependencies
└── README.md                         # This file
```
