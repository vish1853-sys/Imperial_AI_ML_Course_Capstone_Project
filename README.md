# Imperial_AI_ML_Course_Capstone_Project
Capstone project on black-box ML models - building testing and interpreting complex algorithms 

Non-Technical Explanation of the Black Box Optimisation Project 

The Black Box Optimisation project is about finding the best possible inputs to get the best result, without knowing how the system actually works inside.
Think of it as a 'Blind Mountain' challenge where you are trying to find the highest point on a mountain while blindfolded. You can’t see the map, but every time you take a step, a voice tells you your exact altitude.
That is Black Box Optimisation.
We don't know the internal "recipe" or formula of the problem. Instead, we use past results to strategically guess where the next "step" should be. By balancing exploration (trying new areas) and exploitation (climbing known slopes), we find the absolute best outcome using the fewest possible attempts.
DATA

The dataset consists of input-output pairs generated through iterative queries for eight unknown black-box functions.

Inputs: Vectors ranging from 2 to 8 dimensions
Range: All values between 0 and 1
Outputs: Single scalar value representing performance
The dataset grows over time as new queries are submitted in each iteration. No external datasets were used, and all data is generated within the optimisation process.

