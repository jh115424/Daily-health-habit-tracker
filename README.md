# React + Vite

🧠 Core Features to Practice
Storing and updating habits (array of objects)

Toggling a habit as complete/incomplete

Resetting habits daily using date logic

Optional: Save progress in localStorage

🛠️ Main Components
You can build this as a single file for now:

HabitTracker.jsx
Or separate these if you want structure:

HabitList.jsx (renders list)

HabitItem.jsx (one habit box)

App.jsx (manages state and date reset)

- Drink 64oz of Water
- 20-Minute Walk
- Stretch 5 Minutes
- Log Your Mood
- No Sugar Today

---

| Daily Habit Tracker (Header) |
| [Current Date] |

---

| Healthy Meals | Fitness Summary | Water |
| | ---------------- | Intake |
| • Breakfast | • Exercise | • 💧 3L |
| • Lunch | • Intensity | |
| • Dinner | • Duration | |
| | | |

---

===============================
Daily Habit Tracker (Header)  
 [Current Date]  
===============================

[ Healthy Meals ]
• Breakfast
• Lunch
• Dinner

[ Fitness Summary ]
• Exercise: Push-ups
• Intensity: Medium
• Time: 30 mins

[ Water Intake ]
• 💧 3L

===============================

<App>
  ├── <Header />                // Title: "Daily Habit Tracker"
  ├── <DateDisplay />          // Shows current date
  ├── <MealTracker />          // Input or list of healthy meals
  ├── <FitnessTracker />       // Contains:
  │     ├── <ExerciseList />       // List of exercises
  │     ├── <IntensitySelector />  // Light / Moderate / Intense
  │     └── <DurationInput />      // Time in minutes
  └── <WaterIntake />          // Water consumption tracker
</App>

⁡⁢⁢⁣===============================⁡

<App>
  ├── <Header />                // Full-width at the top
  ├── <MainGrid>
        ├── <DateCard />           // Date
        ├── <MealCard />           // Meals logged
        ├── <FitnessCard>          // All fitness info:
        │     ├── <ExerciseList />
        │     ├── <Intensity />
        │     └── <Duration />
        └── <WaterCard />          // Water intake
</MainGrid>
</App>

===============================

Layout 3


------------------------------------------------
|                  HeaderComponent             |
|              "Daily Habit Tracker"          |
------------------------------------------------
|   DateComponent      |   WaterIntakeCard     |
|   [ Today’s Date ]   |   💧 8 Glasses        |
------------------------------------------------
|           HealthyMealsCard (left)           |
|   🥗 Breakfast | 🥪 Lunch | 🍝 Dinner       |
------------------------------------------------
|           FitnessCard (full-width)          |
|   🏋️ Exercise: Pushups                     |
|   🔥 Intensity: Medium                     |
|   ⏱️ Duration: 30 min                       |
------------------------------------------------
|         SummaryFooterComponent (optional)    |
|        "All goals met!" or emoji stats       |
------------------------------------------------


App
│
└── Header               // Title, motivational message, or date
└── MainDashboard        // Main container for all habit cards
    ├── MealsCard        // Healthy meals tracker
    ├── FitnessCard      // Workout log
    │   ├── ExerciseList // Exercise names
    │   ├── Intensity    // Low/Med/High toggle or input
    │   └── Duration     // Time spent on each or total
    └── WaterCard        // Water intake tracker


Suggested Component Structure
HeaderComponent

DateComponent

WaterIntakeCard

HealthyMealsCard

FitnessCard

Optionally: ExerciseInput, IntensitySelect, DurationInput

SummaryFooterComponent (if you want a final daily status)

(Optional: DailyCardWrapper if you want to wrap all daily entries)



Path examples

import FitnessCard from "./Components/FitnessCard/FitnessCard";



Same for subcomponents like:
import ExerciseList from "./Components/FitnessCard/ExerciseList";
