# Final Project ReadMe

For my final project with Flatiron, I wanted to try and create a model that could predict all baseball results. I elected to focus solely on the Philadelphia Phillies for the sake of time. 

# The Goal
Based on historical data, I wanted to be able to analyze the statistics of all baseball games and the final results to try and train my model to be able to predict the next game. 

# The Process
I first had to go through a very vigorous scraping process that involved scraping not only the data of each game for the Phillies, but for all 30 teams in MLB. Once I had all of that data, I had to create seperate data frames for each season of the Phillies with their opponents statistics for every game. This required sorting through all sorts of schedules online manually. 

Once I had all of the data, I wanted to test several models to try and find which one would give me the best results for predicting the games. After trying Logistic Regression and XGBoost, it was clear that XGBoost was superior and had a higher success rate at 56.58% than Logistic Regression at 46.7%. 

With these results, I was able to use the predict_proba function to help accurately predict the % chance of the Phillies either winning the game or losing the game. With these percentages, I was able to create money lines for the game for gambling purposes. For the most part, my numbers were mostly with in a +-30 error compared to the actual books, and that was before even taking into account a human generated advantage for myself. 

# Future Goals
I would love to be able to add more statistics to my model and see if I can get any closer to better predictions. I think also there must be a way I can shorten my code to gather/predict all data for all teams in MLB. This has been a great start, but I would like to really solidify everything about this project.

I have a website ready to go, and the fun part would be to try and make it fully interactive with money lines that have been generated based on my model. Sports gambling is wholly predicated upon statistics, and if I can master the stats of this project I think I can create a fully functional website. 