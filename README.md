# Module 21 Chaallenge

Repository: sms_spam_detector

Files: 
* gradio_sms_text_classification.ipynb  This is the file for the challenge.
* sms_text_classifiation_solution.ipynb  This is the file to refactor or to improve and make the code cleaner and easier to maintain.
* SMSSpamCollection.csv  This is the csv file or dataset located in the Resources foler.
* README.md  This is the current file.
     

## What it does

* Refactor code from the SMS text classification solution.
* Creates two functions: the SMS classification function an the SMS prediction function.
* Create and train the model.
* Create a Gradio interface application.  Users an test 'text messages'.  
* The model will respond whether the text is classified as spam or not.

## Steps
* Refactor the code in the solution file to create a SMS classification function.  Set X or the features variable to text message.  Set y or the target variable to the 'label' column.
* Split into training and testing sets with test_size 0.33
* Pipeline uses TfidVectorizer and LinearSVC.
* Model fitted to the transformed training data and the funtion returns the model.
* The csv file is read into a DataFrame, which is passed to the above fufnction.

* The prediction function has a conditonal statemnt of 'ham' not spam or 'spam.'  It returns the message when called.

* The interface has an input parameter and an output parameter.
* When share=True, a public link is created to access the interface.


## Usage
* Functions
* Pipeline
* Gradio interface application

## Answers to questions
*   1. You are a lucky winner of $5000!
        not spam
    2. You won 2 free tickets to the Super Bowl.
        not spam
    3. You won 2 free tickets to the Super Bowl text us to claim your prize.
        spam
    4. Thanks for registering. Text 4343 to receive free updates on medicare.
        spam
