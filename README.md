# Personalized-Cancer-Diagnosis
2017-KAGGLE ONLINE COMPETITION--  Personalized Medicine: Redefining Cancer Treatment -- Predict the effect of Genetic Variants to enable Personalized Medicine

1. Personalised Medicine-:
- Here personalized Medicine refers to the idea of analyzing an individual patient's tumor to determine what combination of drugs will work best for that particular individual.For doing this, the thousands of genetic mutation in cancer tumor needs to be distinguished into            a. the mutations that contribute to tumor growth (drivers)                                                        
      b.the mutation which are neutral and do not contribute to tumor growth (passengers).             
Since, the interpretation of genetic mutations currently is being done manually.
- So,in this project we automate the classification of these drivers from the passengers.

- Finally our problem statement is - classify genetic variations based on evidence from the text based clinical literature or research papers, which is multi-class classification problem __ because we have 9 classes.

2. DataSet Overview:
- There are nine different classes a genetic mutation can be classified on. Both, training and test data sets are provided via two different files. 
- One (train_variants) provides the information about the genetic mutations, whereas the other (train_text) provides the clinical evidence (text) that our human experts used to classify the genetic mutations. Both are linked via the ID field. 

3. Business objectives & constraints-:
   1. Interpretability of the algorithm is must because, at the end doctor or specialist should understand why our model predicted that      class.                 
   2. No low-latency requirement which means patient can wait few minutes for results. This tells us that we can use complex models.
   3. Errors can be very costly : We should not live with errors , as we are dealing with lives of patient.
   4. Probabilities of data point to each class needed because, if two classes have somewhat similar probabilities,doctor may suggest        patient to go with more tests.

4. Performance metrics used -- Multi class Log-Loss , Confusion matrix
   - (Log-Loss is chosen because it actually uses probability which is our business constraint)

5. Machine Learning objective: Predict the probability of each data point belonging to each of nine classes.
