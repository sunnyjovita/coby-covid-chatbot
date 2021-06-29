# coby-covid-chatbot
# How the program works

- To see and use our code please download all the resources on  Github  link  provided  in  the  supplementary  files.  
- Install all  the  libraries  required  and  then  install  Telegram.  
- The  usermanual is provided in the Github. 
- The application can be added to  the  Telegram  by  search  thecoby_chatbot application name.

<img width="425" alt="telegram search" src="https://user-images.githubusercontent.com/55756082/123628304-22992a80-d83d-11eb-9722-a93c33bf9c26.png">

- After getting the intents or tags from the algorithm, we usehandler to pick the output for the bot.

- Figure 6
<img width="353" alt="handler" src="https://user-images.githubusercontent.com/55756082/123628488-5a07d700-d83d-11eb-8565-ac3a2c548d01.png">

- Figure 7
<img width="526" alt="switch" src="https://user-images.githubusercontent.com/55756082/123628540-67bd5c80-d83d-11eb-8a21-54f0f4366e20.png">

- There  is  a  variable  switch  that  is  a  dictionary  that  giveseach tags a value to call their own function (Figure 7).
- Each  function  have  their  own  type  of  outputs,  there  aresome that uses web scrapper (Figure 8), some uses the requests (Figure 9), and some that uses custom outputs (Figure 10).
- Figure  8  is  a  web  scraper. 
- To  create  a  web  scraper  youneed  to  know  the  layout,  the  contents  of  the  page,  and  theHTML  tags. 
- How  it  works  is  that  it  search  the  tags  insidethe  HTML  body,  and  for  this  particular  one,  first  we  searchfor the tag h2 that have the value of ”Watch for Symptoms”, next grab a paragraph and also a unsorted list (Limit indicatehow much of the certain tag should they get).

- Figure 8
<img width="701" alt="web scrapper" src="https://user-images.githubusercontent.com/55756082/123628793-b3700600-d83d-11eb-9407-ca96d0e5561f.png">

- Figure 9
<img width="875" alt="requests" src="https://user-images.githubusercontent.com/55756082/123628814-b79c2380-d83d-11eb-847b-1f1c642496a7.png">

- Figure 9 Requests is one of the way to get an API, it worksalmost  the  same  as  fetch()  API  on  JavaScript. 
- This  one  isused to get the updated data of COVID-19 so the output couldalways  send  the  updated  information  each  time  user  ask  thequestion.

- Figure 10
<img width="612" alt="costume" src="https://user-images.githubusercontent.com/55756082/123628842-bff45e80-d83d-11eb-96e0-f34800afd97f.png">

# Models
- SVM (Support Vector Machine with scikit-learn)
- NN (Neural Network)
- NB (Naive Bayes)

# Data : dataset.tsv (train.tv 66%, test.tsv 33%)
- Training data: train.tsv
- Testing data: test.tsv

# Bot
- Find me on telegram t.me/coby_chatbot.

# Video
- https://youtu.be/aiUFY9W1SgA

# Requirements
- NLTK
- Scikit-learn  (and  their  dependencies)
- Torch
- Selenium
- Beautifulsoup4
- Python-telegram-bot
- Requests
- Pycountry

# Run the program
- run telegram_main.py after you install all the python libraries
