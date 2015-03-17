# Problem
We want to see if we can make an algorithm to create an entirely new song.

# Question
1. How can we implement machine learning?
2. How can an accompaniment be created?
3. How can a melody be created?

# Resources
1. [Machine Learning]
2. [Chord Progressions]
3. 

### 1. How can we implement machine learning?
No matter how the program creates the song, it will have to have some way to determine if the song is "good". After the algorithm has been written, a number of songs must be created, listened to by humans, and classified as good or bad. After this has been done, each song must be analyzed by the computer and given a few values determined by attributes of the song. By graphing each of the songs with the values given, you can begin to form a plane through the graph that seperates good songs from bad songs. After a threshold has been found, the program can now compare any new songs it makes to songs that were considered "good" and determine if it has created a song that sounds good. It is important to note that although there are many algorithms available to find the threshold between good and bad results, they all essentially do the same thing so getting large amounts of data is the most important step in this process.

This resource answers the question 1: how can we implement machine learning?

### 2. How can an accompaniment be created?

One of the simplest accompaniments possible is a chord progression. By randomly selecting a key, or allowing the user to input a key of their choise, it is simple enough to create a progression of chords. According to [Chord Progressions], finding the euclidean distance between the attributes of two different chords results in variables that represent how similar the two chords are. These variables can then be converted into probabilities of substitution between chords and used to determine how likely it will be that one chord will follow another. I can use these probabilities to randomly generate a series of chord progressions that will serve as the accompaniment to the song.

This resource answers question 2: how can an accompaniment be created?

### 3. How can a melody be created?

This resource answers question 3: how can a melody be created?

[Machine Learning]: http://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf
[Chord Progressions]: http://ismir2005.ismir.net/proceedings/1091.pdf
[The Echonest]: http://the.echonest.com/
