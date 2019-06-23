This guide refers to developing a Neural Network capable of predicting results of matches. There have been attempts before in creating a Neural Network that learns over games to predict outcome of rain affected matches.

https://people.ucsc.edu/~praman1/static/pub/ML_Project_CS7641.pdf

Above, only takes in 52 matches. Too less for a neural network to train on. We will gather data for a thousand matches (a humungous task that will alone take months).
And then train the network. Matches not affected by rain will be considered at several stages.

Flaws with the Duck-Worth-Lewis-Stern Method:
  Ok the problem with the DWLS method is that it doesn't take into account the quality of batsmen remaining, the quality of pitch (high-scoring or low-scoring) and doesn't take into account recent trends (300 plus chases are common these days).
  
  Our input is going to be like the following from a match lost:
  
  ENGvsAUS
  
  Input tensor:
  
  115,96,4.75,4,.......,LOSS
  
  Categories:
  
  Runs to get, balls left, current run-rate, wickets left, (Averages and past 3 performances of batsmen upto 11), WIN/LOSS
  
  
  
  

