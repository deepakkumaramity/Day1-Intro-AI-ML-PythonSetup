# Day1-Intro-AI-ML-PythonSetup
# Day 1 – Gym Routine Dataset
# Author: Deepak Kumar

import pandas as pd
import numpy as np

# Creating a simple dataset
data = {
    'Day': ['Mon', 'Tue', 'Wed', 'Thu', 'Fri'],
    'Exercise': ['Chest', 'Back', 'Legs', 'Arms', 'Shoulder'],
    'Duration': [90, 85, 95, 80, 100]
}

df = pd.DataFrame(data)

print("🏋️ Gym Routine Dataset (Deepak Kumar):")
print(df)

# Calculate average duration
avg_duration = df['Duration'].mean()
print("\n📊 Average Duration:", avg_duration)

# Extra Analysis
print("\n🔹 Max Workout Day:", df.loc[df['Duration'].idxmax()])
print("🔹 Min Workout Day:", df.loc[df['Duration'].idxmin()])
