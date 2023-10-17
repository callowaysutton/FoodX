# Artificial Intelligence Work Prompt

## FoodX Background

One of the biggest aspects of the Xtern program is showing off our wonderful state and all it has to offer. Indiana is not only home to amazing sites and attractions, but also several local and unique dining options, like Food Trucks. TechPoint is excited to help amplify the Indiana Food Truck scene and will open our very own FoodX franchise and we need your help! In order to spread the Food Truck love, you will be asked to help develop the concept of amplifying the food truck scene in Indiana and helping to launch the franchise, FoodX.

#### Your Task

In the next section, you will be given your corresponding responsibilities for the amplification of the Indiana Food Truck scene and/or the launch of the food truck franchise. Read each task carefully and ensure you submit your work by the deadline!

Disclaimer: The above description is fictional.  The TechPoint team does not have an app or a food truck and is not using your work sample assessment to finalize features of it.  Any work completed will be used for the application to the Xtern internship.

#### Situation

Given the launch of our food truck line, FoodX, we will be running an exciting and interactive promotion on college campuses to attract a massive initial student following. When placing their order on our fancy new FoodX app they input basic information about their college experience and we predict what they are going to order. If we don’t get it right they get a 10% discount.

While the promotion has done a great job of bringing in business our staff has not been great at guessing orders and are not happy with the combined workload of guessing and cooking.

Because of this you have been asked to consider implications, solutions and deployment of a mechanism to automatically guess orders, sounds like the perfect job for AI!

### (25%) Given the data set, do a quick exploratory data analysis to get a feel for the distributions and biases of the data. Report any visualizations and findings used and suggest any other impactful business use cases for that data.

#### This is found in exploring_the_data.ipynb

### (30%) Consider implications of data collection, storage, and data biases you would consider relevant here considering Data Ethics, Business Outcomes, and Technical Implications

#### This is found in Implications.md

### (35%) Build a model to predict a customers order from their available information. You will be graded largely on your intent and process when designing the model, performance is secondary. It is strongly suggested that you use SKLearn for this model as to not take too much time. You may use any kind implementation you would like though, but it must be pickelable and have a “.predict()” method similar to SKLearn

#### This is found in model_to_predict_order.ipynb and model_to_predict_order_time.ipynb (this one was just out of curiosity)

### (10%) Given the work required to bring a solution like this to maturity and its performance, what considerations would you make to determine if this is a suitable course of action?

#### I would make sure that the company has the infrastructure and ability to handle the load for inferencing new data before even thinking about deploying it first and foremost. Not to mention I would try to make very scrutinous tests that go through the dataset and check for any biases as well as make sure there is a diverse enough amount of data that the dataset reflects real world values. For example, I would not deploy this dataset into a business critical, or even non critical, application since it doesn't seem to reflect real world values reliably and misses a lot of useful information such as geographic location of the resturaunts, name of the resturaunts, majors outside of STEM, other grades besides 2nd and 3rd years, etc.

#### Some considerations I would make for determining when this dataset is ready for market is when it shows a very diverse set of different data points to where it can accurately guess what a college student would want off the time, their school, major and year at around or above 90% of the time at a minimum. Below this would be far too risky to use in any application where revenue could be risked in my opinion.