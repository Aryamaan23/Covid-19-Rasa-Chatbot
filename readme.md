## Covid-19 RASA Chatbot

## About Covid-19
![corona-1](https://user-images.githubusercontent.com/60667917/95548547-f4f82100-0a22-11eb-95f6-95785999bd37.jpg)

## What Is COVID-19?
A coronavirus is a kind of common virus that causes an infection in your nose, sinuses, or upper throat. Most coronaviruses aren't dangerous.

In early 2020, after a December 2019 outbreak in China, the World Health Organization identified SARS-CoV-2 as a new type of coronavirus. The outbreak quickly spread around the world.

COVID-19 is a disease caused by SARS-CoV-2 that can trigger what doctors call a respiratory tract infection. It can affect your upper respiratory tract (sinuses, nose, and throat) or lower respiratory tract (windpipe and lungs).

It spreads the same way other coronaviruses do, mainly through person-to-person contact. Infections range from mild to deadly.

SARS-CoV-2 is one of seven types of coronavirus, including the ones that cause severe diseases like Middle East respiratory syndrome (MERS) and sudden acute respiratory syndrome (SARS). The other coronaviruses cause most of the colds that affect us during the year but aren’t a serious threat for otherwise healthy people.

## Corona Symptoms
![corona-2](https://user-images.githubusercontent.com/60667917/95548913-b9118b80-0a23-11eb-91ae-c50d9d256a02.jpg)

Symptoms of COVID-19
The main symptoms include:

1.Fever 
2.Coughing
3.Shortness of breath
4.Trouble breathing
5.Fatigue
6.Chills, sometimes with shaking
7.Body aches
8.Headache
9.Sore throat
10.Congestion/runny nose
11.Loss of smell or taste
12.Nausea
13.Diarrhea

## What to do if you think you have it
If you live in or have traveled to an area where COVID-19 is spreading:

If you don’t feel well, stay home. Even if you have mild symptoms like a headache and runny nose, stay in until you’re better. This lets doctors focus on people who are more seriously ill and protects health care workers and people you might meet along the way. You might hear this called self-quarantine. Try to stay in a separate room away from other people in your home. Use a separate bathroom if you can.
Call the doctor if you have trouble breathing. You need to get medical help as soon as possible. Calling ahead (rather than showing up) will let the doctor direct you to the proper place, which may not be your doctor’s office. If you don’t have a regular doctor, call your local board of health. They can tell you where to go for testing and treatment.
Follow your doctor’s advice and keep up with the news on COVID-19. Between your doctor and health care authorities, you’ll get the care you need and information on how to prevent the virus from spreading.

## About Rasa
![rasa](https://user-images.githubusercontent.com/60667917/95549588-2f62bd80-0a25-11eb-8fae-22abbb2307d2.jpg)

Rasa is an open source machine learning framework for automated text and voice-based conversations. Understand messages, hold conversations, and connect to messaging channels and APIs.

## Build your assistant
In this guide, we are creating an assistant that helps users subscribe to a newsletter. Go through each of the steps below to see how a simple assistant is created:

1. NLU data

What are the various things people might say to an assistant that can help them subscribe to a newsletter?

For an assistant to recognize what a user is saying no matter how the user phrases their message, we need to provide example messages the assistant can learn from. We group these examples according to the idea or the goal the message is expressing, which is also called the intent. In the code block on the right, we have added an intent called greet, which contains example messages like “Hi”, “Hey”, and “good morning”.

Intents and their examples are used as training data for the assistant's Natural Language Understanding (NLU) model.

2. Responses

Now that the assistant understands a few messages users might say, it needs responses it can send back to the user.

“Hello, how can I help you?” and “what’s your email address?” are some of the responses our assistant will use. You’ll see how to connect user messages and responses in the next steps.

In the code block below, we have listed some responses and added one or more text options for each of them. If a response has multiple text options, one of these options will be chosen at random whenever that response is predicted.

3. Stories

Stories are example conversations that train an assistant to respond correctly depending on what the user has said previously in the conversation. The story format shows the intent of the user message followed by the assistant’s action or response.

Your first story should show a conversation flow where the assistant helps the user accomplish their goal in a straightforward way. Later, you can add stories for situations where the user doesn't want to provide their information or switches to another topic.

In the code block below, we have added a story where the user and assistant exchange greetings, the user asks to subscribe to the newsletter, and the assistant starts collecting the information it needs through the newsletter_form. You will learn about forms in the next step.

4. Forms

There are many situations where an assistant needs to collect information from the user. For example, when a user wants to subscribe to a newsletter, the assistant must ask for their email address.

You can do this in Rasa using a form. In the code block below, we added the newsletter_form and used it to collect an email address from the user.

5. Rules

Rules describe parts of conversations that should always follow the same path no matter what has been said previously in the conversation.

We want our assistant to always respond to a certain intent with a specific action, so we use a rule to map that action to the intent.

In the code block below, we have added a rule that triggers the newsletter_form whenever the user expresses the intent “subscribe”. We’ve also added a rule that triggers the utter_subscribed action once all the required information has been provided. The second rule only applies when the newsletter_form is active to begin with; once it is no longer active (active_loop: null), the form is complete.

Learn more about rules and how to write them.

Now that you've gone through all the steps, scroll down to talk to your assistant.

## Rasa Chatbot
This bot gives the statistics of corona cases statewise and it also gives the basic information about corona and its symptoms.
