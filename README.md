 Cricket Pitch Behavior Clusterer
A machine learning project that analyzes and categorizes cricket stadium pitches based on their playing characteristics using K-means clustering.
---- Project Overview
This project groups cricket pitches into distinct categories by analyzing historical match data. It helps understand pitch behavior patterns across different stadiums, which is valuable for:

Team strategy planning
Stadium groundskeeping optimization
Match outcome prediction
Player selection decisions

---- Pitch Categories
The model classifies pitches into four distinct types:

Batting Paradise - High-scoring grounds favoring batsmen
Pacer's Heaven - Pitches that assist fast bowlers
Spinner's Delight - Surfaces supporting spin bowling
Unpredictable Pitch - Balanced or variable conditions

---- Features Used
The clustering algorithm analyzes four key metrics:

Average Score: Typical runs scored at the venue
Pace Wicket %: Percentage of wickets taken by fast bowlers
Spin Wicket %: Percentage of wickets taken by spinners
Boundary Rate: Frequency of boundaries (4s and 6s)

---- Technologies Used

Python 3.x
pandas: Data manipulation and analysis
scikit-learn: K-means clustering and data preprocessing
matplotlib: Data visualization

---- Methodology

Data Loading: Import stadium pitch data from CSV
Data Cleaning: Handle missing values and convert to numeric format
Feature Scaling: Standardize features using StandardScaler
Clustering: Apply K-means algorithm with 4 clusters
Visualization: Generate scatter plots for pattern analysis
Output: Export clustered results to CSV

---- How to Run
Prerequisites
bashpip install pandas matplotlib scikit-learn
Execution

Clone the repository
Update the CSV file path in the code:

python   df = pd.read_csv("path/to/your/stadium_pitch_data.csv")

Run the script:

bash   python Stadium_pitch.py
📁 Input Data Format
Your CSV should contain the following columns:
ColumnDescriptionStadiumName of the cricket stadiumAvgScoreAverage score at the venuePaceWicket%Percentage of wickets by pace bowlersSpinWicket%Percentage of wickets by spin bowlersBoundaryRateRate of boundaries scored
📈 Output
The script generates:<img width="1527" height="827" alt="Screenshot (93)" src="https://github.com/user-attachments/assets/b9ad6d6f-0bb3-4db1-8a26-9fb487e8e333" />


Console Output: Clustered stadium classifications
Visualizations:

Pace vs Spin wicket percentage scatter plot <img width="750" height="607" alt="Screenshot 2025-12-05 172633" src="https://github.com/user-attachments/assets/f4651290-beee-422f-90b4-9c1a16e0f84d" />

Average Score vs Boundary Rate scatter plot <img width="777" height="591" alt="Screenshot 2025-12-05 172702" src="https://github.com/user-attachments/assets/d6376187-45fe-46c3-89cb-db37c2878332" />



CSV File: pitch_clustered_output.csv with cluster assignments

🔍 Sample Output
Stadium                Pitch_Type
----------------------------------
Wankhede Stadium      Batting Paradise
Eden Gardens          Spinner's Delight
Lord's Cricket Ground Pacer's Heaven
...
📊 Visualizations
The project creates two key visualizations:

Pace vs Spin Analysis: Shows the bowling characteristics of each pitch
Scoring Pattern Analysis: Reveals the relationship between scores and boundary frequency

🎓 Learning Outcomes

Unsupervised learning with K-means clustering
Feature engineering for sports analytics
Data preprocessing and scaling techniques
Sports data visualization

🔮 Future Enhancements

 Add weather and seasonal conditions as features
 Implement elbow method for optimal cluster selection
 Include pitch deterioration patterns (Day 1 vs Day 5)
 Add interactive visualizations using Plotly
 Incorporate team performance metrics

📝 License
This project is open source and available under the MIT License.
🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
👨‍💻 Author
Your Name - Sruthi-1601
