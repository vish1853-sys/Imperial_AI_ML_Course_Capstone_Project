# Imperial_AI_ML_Course_Capstone_Project
Capstone project on black-box ML models - building testing and interpreting complex algorithms 

Non-Technical Explanation of the Black Box Optimisation Project 

The Black Box Optimisation project is about finding the best possible inputs to get the best result, without knowing how the system actually works inside.
Think of it as a 'Blind Mountain' challenge where you are trying to find the highest point on a mountain while blindfolded. You can’t see the map, but every time you take a step, a voice tells you your exact altitude.
That is Black Box Optimisation.
We don't know the internal "recipe" or formula of the problem. Instead, we use past results to strategically guess where the next "step" should be. By balancing exploration (trying new areas) and exploitation (climbing known slopes), we find the absolute best outcome using the fewest possible attempts.


DATA (See Datasheet_Capstone) Datasheet_Capstone

The dataset consists of input-output pairs that is generated through iterative queries for eight unknown black-box functions.

Inputs: Vectors ranging from 2 to 8 dimensions
Range: All values between 0 and 1
Outputs: Single scalar value representing performance
The dataset grows over time as new queries are submitted in each iteration.  All data is generated within the optimisation process without any external involvement.

MODEL (See Model_card_Capstone) Model_Card_Capstone

This project does not rely on a single predefined machine learning model. Instead, it uses an iterative, pattern-based optimisation approach.

Key ideas include:

Identifying high-performing regions (clusters)
Observing directional trends across iterations
Refining solutions using smaller adjustments
This approach was chosen because of limited data, uncertainty in function behaiour and the need for interpretability. 


Hyperparameter Optimisation 

Rather than tuning model hyperparameters, the optimisation focused on:

Step size of parameter changes
Balance between exploration and exploitation
Selection of candidate regions for refinement
Early rounds used larger variations (exploration), while later rounds used smaller, controlled adjustments (exploitation).

Outcome (See Juptyer notebook BBO_capstone.jpynb) BBO_Capstone.ipynb

The optimisation process showed:

Improvements in early rounds for some functions 
Identification of stable high-performing regions
Diminishing returns in later rounds for some functions 

Key findings:

High-performing inputs form clusters, especially for high dimensional functions. 
Some dimensions influence results more strongly and early exploration significantly impacted the final results.
