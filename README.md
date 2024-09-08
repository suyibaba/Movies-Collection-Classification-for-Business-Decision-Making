# Movies-Collection-Classification-for-Business-Decision-Making


              ## Business Case
              
              
              1. A 506 rows of movie production details was generated for a movie production company with the aim of predicting and understanding the impact various       
              variables have on determing the collection values so the organization can know how to distribute there resources thus, improving the collection and 
              profits to be made for each class of movie production. 
              2. Objective two is to know if the movie will win an Award at the movies show
              3. Compare the models and look for ways to get the best models and apply them 
              
              
              
              
              
      ## METHOD OF ANALYSIS AND PREDICTION 
      
      
      
            1. A Decision Tree method and algorithm was used for the prediction for objective one
            2. Classification Tree was used to achieve objective two
            3. Bagging and Random Forest techniques will be used to analyse the Data so as to give a deductive comparison with Decision tree model and Classification Tree model. 
            
            
                              OBJECTIVE ONE
        ##  DETAILS AND RESULTS
        
        
        1. Data Preprocessing 
        2. Treating Missing Values
        3. Dummy Variable Creation :  #convert all our categorical variables into numerical variable by using dummy variables
                                      #dummy variable is 1 minus number of categories
        4.  X-Y SPLIT
        5. Test and Train Split
        6. Training Regression Tree : #maxtree(max_depth = number of layers in my tree)
        
        
        
        
          ##  MODEL PERFORMANCE
          
         r2_score for train dataset = ##  0.8365
         
         r2_score for test dataset = ## 0.6541
         
         #r2 for train dataset is showing bigger than test data set because we have trained our model on our train dataset and it will always perform better on the     dataset of which it was trained.
         
         
         ###Plotting decision tree
         


![image](https://user-images.githubusercontent.com/64482231/192121806-343916eb-ff4c-4c5d-9ac7-37a31dcceec2.png)









X[3] REFERS TO THE fourth varaible of the X dataset, 37982.312 = the condition, if the budget is less than thirty seven thousand, then it will follow the true branch and vice versa.
#the total number of observation is 404    
         



              Controlling Tree growth
              
              
       # Maximum number of levels in tree
       
![image](https://user-images.githubusercontent.com/64482231/192121858-e3cdb412-11ec-4666-8674-8241998634ce.png)











        Mininum observations at internal node
        
        
        
![image](https://user-images.githubusercontent.com/64482231/192121869-7054c377-02f8-49c7-887a-09bb749375a6.png)









      ## minimum observations at leaf node
    
    
![image](https://user-images.githubusercontent.com/64482231/192121880-257dffaf-93d6-4a95-9418-8dfefbaaf83e.png)





                                                  OBJECTIVE TWO
                                                  
                                   ***Predicting the movies winning an award
                                   
![image](https://user-images.githubusercontent.com/64482231/192124371-538acba6-5f85-4fd9-8c1d-c7cab2764430.png)




              Controlling tree growth
              
      
      
![image](https://user-images.githubusercontent.com/64482231/192124394-6887ab59-0135-4b47-ba0d-cb0ce59c894a.png)



                                        OBJECTIVE THREE
                                        
                                        
        1.  BAGGING/ENSEMBLE TECHNIQUE              
        
        
         confusion_matrix
         array([[27, 17],
                [22, 36]], dtype=int64)
                
         accuracy_score
         0.6176470588235294
         
         
         
         #by comparing the accuracy with the previous models 

          #Bagging = 61.76 percent
              # Single Decision tree = 54.9 percent
                  #Decison Tree after prunning = 55.8 percent

        #Creating large number of tress increased the accuracy
        
        
        
        
        2. Random Forest 
        
        
        
        confusion_matrix
        
        
        array([[25, 19],
               [18, 40]], dtype=int64)
               
               
       accuracy_score
       
       0.6372549019607843
       
       
       #by comparing the accuracy with the previous models 

                #Bagging = 61.76 percent
                # Single Decision tree = 54.9 percent
                #Decison Tree after prunning = 55.8 percent
                #RandomForest = 63.73 percent
                
                
        3.  Using XgBoost
        
        
![image](https://user-images.githubusercontent.com/64482231/192919937-b30001e0-f558-499a-b584-a28e6b3a8ff4.png)



 accuracy_score
       
       0.5980392156862745
