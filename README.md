# Song-Recommendation Using AI-and-Digital-Signal-Processing

## Music Audio Digital Signal Processing, Genre Classification and Recommendation

## This project aims to classify and recommend songs using acoustic features, extracted by digital signal processing methods and convolutional neural networks. Study has been conducted over two steps; determining how features that will be used in recommendation are obtained and developing a service that recommends songs to user requests. Firstly, feature extraction has been carried out by means of digital signal processing methods and then CNN has been trained as an alternative feature extraction. Then acoustic features of songs are used in classification to determine the best neural network architecture, which would give the best genre prediction and hence, best recommendation results. 

## After finding the best CNN network architecture, which gives 70-75% accuracy for genre prediction on data it has never seen before, I made a 3 dimensional predictions array in which I stored the genre prediction values of each song. This would be the representation of each song in our dataset, a numpy array consisting of the different probabilities of genres our network thinks, the song is, essentially, a vector.

## Now, for a given song, we first take its prediction array, and find out its Euclidean distance with each of the other song vectors. The top 5 songs are selected for recommendation, which are nearest to the given song i.e least Euclidean distances. Our model recommends songs well, finding out the most similar songs to a given, in that particular genre. 

## This approach to song recommendation can enable users discover new genres of music, as, every song can actually be thought of as a collection of different genres. This method does not rely on data about what other people are listening to, and make user profiles, instead, it directly analyses the song’s signal and recommends similar songs. This can enable new artists’s good music reach people who might find it suiting to their tastes, as these artists might not get the reach, due to less popularity. 
