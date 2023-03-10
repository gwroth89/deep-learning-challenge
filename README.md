# deep-learning-challenge
The purpose of this analysis was to create a binary classifier model to predict the success of charity applications based on several provided features.


Data Preprocessing

As shown below, I used the IS_SUCCESSFUL column as my target and all other columns as features in my initial model. I removed EIN and NAME from the dataset as they were just identifiers and not features that should impact the model.
![image](https://raw.githubusercontent.com/gwroth89/deep-learning-challenge/main/images/Screen%20Shot%202023-03-09%20at%203.57.32%20PM.png)

Compiling, Training, and Evaluating the Model

- In both my initial and optimized models, I used 3 layers. I found that increasing beyond that decreased the stability of the model, especially if I added more parameters. In my initial model, I tried 2 but found better performance with the third.
- In my initial model, I started with 110 Neurons, in the optimized model I ran with 7 and saw little difference in performance. This was somewhat surprising, indicating that to a degree, a less is more approach can work.
- I was unable to reach target performance, despite taking the steps below to improve my model

Model Optimizations:
- Remove unnecessary features: I dropped several columns from the model that seemed to have little bearing on outcome 
- Reduced neurons: I tried reducing here as I noticed a substantial drop in accuracy/stability in my optimized notebook. By reducing neurons, I was able to match my original performance. Sometimes adding too many appears to add instability/noise to the model.
- Rearranged activation layers: I tried rearranging my activation layers but found the most success keeping ReLu as my input layer in both models.
