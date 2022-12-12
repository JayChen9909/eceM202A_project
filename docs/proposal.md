* Motivation & Objective

The beginners of playing instruments are always trying to improve their performance based on the expression of emotions. However, it is not possible for them to directly consult the masters who play pretty well in emotional expression of instruments, and it is not easy to even learn from them based on only watching or listening. In this case, it is better for learners to clearly understand what and how hard their emotions are during playing with a digital data standard and feedback. In this project, I collected the motion data of the accelerometer on Arduino Nano33 BLE board while the professional musicians are playing different instruments. According to the main categories of music instruments that can be summarized as four types: Keyboard, Wind instrument, Percussion and String, I chose one representative instrument for each of them to collect and analyze, which are Piano, Clarinet, Drum and Violin respectively. In order to ensure the data is trustworthy, I invited the players from UCLA Herb Alpert School of Music to play the instruments respectively, who major in the corresponding instruments. And due the trained model from those data through the Edge Impulse, I deployed the classifiers onto the Nano33 BLE board that are able to do the live classification. The future application for this project is assumed to be an instrumental training helper that assists musicians to practice their performance of emotion expression with clear and understandable feedback. 

* State of the Art & Its Limitations: 

Most of the currently existing research mainly focus on music genre classifications, which analyze the music features extracted from the audio signal information. However, the research toward emotion analysis is few, and the emotion analysis based on motion from instrument players is almost none. In this case, this project is very worth doing to check whether the classification model built on motion data would perform better or not. 

* Novelty & Rationale: 

After reading the state-of-art in researching musical emotion analysis, the accelerometer of the kinetic sensor is chosen to catch the information details of music players’ motions, which would extract the motion information through the acceleration changes in different dimensions (x, y, z). For the novelty, the first thing is I use the accelerometer data to go through the neural network for learning the motion features to further classify the emotions from them as the results in this area are still unclear. The second point is I will compare the performance of classifiers from four main categories of instruments, which are represented by Piano (Keyboard), Clarinet (Wind), Violin (String) and Drum (Percussion), and try to find out if there is any common phenomenon that requires further research in the future. The last point is that I will apply the trained classifier onto the Arduino Nano33 BLE as a rough demo of application of this project in practical situations. 

* Potential Impact:

From the practical situations, this project offers the results in music emotion classification in the direction of motion data, which would further contribute to more multidisciplinary research to better improve the neural network model designs for higher classification accuracy. And from the ideal situations, it is expected to become the efficient helper product for the beginners of music instruments to improve their emotion expression in performance. 

* Challenges: 

The risk is that before starting this project, I am not sure if the results would be better than the popular method of using audio signals to classify music emotions, which means the classification performance would be even worse than the previous research. And the challenge for this project is, in order to make the results of classifiers to be as trustworthy as possible, I need to strictly ask the performers to play as accurate as possible, and the data should be as more and as various as possible, which would be difficult to design this project with the period of only one quarter of study. 

* Requirements for Success: 

For the resource of data collected in this project, the requirements mainly focus on the musical instruments performers. It requires the professional players to play a series of music that accurately corresponds to the directions of emotion from the researcher. 

For the skills required from this project, it can be mainly concluded by the software part and hardware part. The software part requires the researcher to learn how to use the Edge Impulse to build the correct model with a series of parameters settings and block choices, and how to compare the models with different settings for picking the best model to further deploy. The hardware part requires the researcher to learn how to use Arduino Nano33 BLE board by flashing firmware of model onto the board and how to run the model for live test. 

* Metrics of Success:

In this project, the metrics of success are mainly based on the output of classification accuracy of the models based on different instruments data, which can be checked through two ways: The first way is the model evaluations on Edge Impulse. According to the function of Edge Impulse, it is able to run the self-validations based on the split data for tests, and the accuracy of classifying each emotion would be illustrated from a summarized confusion matrix. The second way is the live test on Arduino Nano33 BLE board. By correctly running the model on the Nano33 BLE board, a live test would keep running and refreshing the real-time classification of the emotions, which give the feedback in the form of percentages to emotions repsectively, and higher percentage indicates a more possible emotion that the player is expressing.
