# Feltz_Penn_DataChallenge

Attached, please find my Jupyter Notebook containing the code for the predictive model. Notebook is titled: Feltz_PI_DataChallange.ipynb

Below are answers to several of the question prompts:


•	If you used a different model, why'd you choose this model? What about it made it work for this problem? Is this model complex and if so, is the complexity necessary? Is it intuitive enough to explain it to a lay-person? What was your optimizing metric? What were the hyperparameters and why'd you choose them?

-I chose to stick with the same LSTM neural network that was used. Because the business case was to predict future values based on sequential data in the past, the LSTM is a good choice. However, I chose to create my own model and code versus changing the model and debugging the given code. It was a personal preference to start from scratch so that I could have a blank slate and be able to code as I preferred rather than trying to work with what was already given. Because LSTM models are sensitive to the scale of the input data, I needed to make sure that I scaled/normalized my data to a range of 0-1. This way, my model does not weight the features unequally, otherwise some features could be falsely prioritized/weighted over other features in the representation. I then broke my data into a training and test set with a 70/30 split, and changed the shape of my data in order to match the input format needed for a LSTM model. I chose to use the learning rate of 0.001 after trying multiple different values because the 0.001 learning rate produced the best results. I used ADAM as my optimizing metric because I wanted to be able to train my model in less time and more efficiently; therefore, ADAM was the best optimizer to choose.


•	Did you include any regularization strategies in your model? If so, why'd you choose the one you did?

-Yes, I did include regularization strategies in my model. I chose to include the dropout regularization method in order to reduce overfitting and to improve model performance.


•	Did you include visualizations? (everyone loves a good graphic)

-I included several visualizations throughout the process. First, I created a visualization to see the trend of the price for the entire given data set. I also included visualizations at the end in order to visually see the model’s performance with the comparison of the actual data verses the model’s predictions. I like to include visualizations in my work, not only for my own benefit, but also for the benefit of my stakeholder/customer. When explaining a model and its performance to others, especially individuals that do not have a technical or data science background, I have found that visualizations are a great addition in helping to make the explanation clearer and easier to understand.
