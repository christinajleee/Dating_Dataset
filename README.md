Background and Motivation

As online dating becomes an increasingly common way to form relationships, I wanted to better understand the factors that drive success on these platforms. For this project, I used an artificial dataset generated from Kaggle that simulates dating app behavior and usage. The dataset contains 50,000 records and 19 variables covering user demographics, profile details, and behavioral patterns.
My primary goal was to analyze both algorithmic and behavioral factors that influence matching success on dating apps. Beyond academic interest, this project has practical applications for improving user experience and platform design for current and future dating apps.

Data and Variables

The dataset included a wide range of variables, such as:
- Demographics: gender, age, sexual orientation, education level, income bracket, height, weight, zodiac sign, body type, relationship intent
- Profile characteristics: profile picture count, bio length, interest tags, profile completeness
- Behavioral factors: swipe right ratio, app usage time, likes received, mutual matches, message count, emoji usage, swipe time of day
- Outcomes: match outcome (success vs. not)

Methods

I began with exploratory data analysis to identify correlations and baseline success rates. Initial findings showed relatively flat success rates and limited variation across demographic groups. I then applied Bayesian logistic regression to estimate how different factors influenced the likelihood of a successful match. Finally, I tested an ensemble classification model, which outperformed the individual models in predictive accuracy.

Results

- Bayesian Logistic Regression
  - Factors that increased success: app usage time, swipe right ratio, and profile completeness.
  - Factors that decreased success: excessive profile pictures, longer bios, and certain demographic variables.
  - Overall performance: test accuracy of 74.7% against a base success rate of 25.3%.
- Ensemble Model
  - Achieved 81.2% test accuracy and 0.830 AUC, outperforming individual classifiers.
  - Precision for predicting successful users was 0.79, while recall was lower at 0.35, indicating a conservative but reliable prediction strategy.
  - Weighted average F1-score of 0.78, demonstrating consistent performance.

Key Insights

- Success is less about demographics or physical attributes and more about behavioral strategy.
- The strongest predictors of success included:
- Being selective in swiping
- Moderate but consistent app usage
- Having 3–4 profile pictures (not too few, not too many)
- An optimal bio length (neither too short nor too long)
- Higher engagement (sending messages, using emojis thoughtfully)
- Demographic factors such as age, gender, education, and income had minimal impact, while height and weight showed weak correlations.

My findings suggest that thoughtful, balanced engagement with the platform leads to better outcomes than relying on inherent characteristics. The most successful users are selective and intentional in how they interact, rather than swiping indiscriminately or remaining overly passive.
