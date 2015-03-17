# Problem
We want to see if we can make an algorithm to create an entirely new song.

# Question
1. How can we implement machine learning?
2. How can we create an accompaniment?
3. How can we create a melody?

# Resources
1. [Machine Learning]
2. [Chord Progressions]
3. [Music and AI]

### 1. How can we implement machine learning?
No matter how the program creates the song, it will have to have some way to determine if the song is "good". After the algorithm has been written, a number of songs must be created, listened to by humans, and classified as good or bad. After this has been done, each song must be analyzed by the computer and given a few values determined by attributes of the song. By graphing each of the songs with the values given, you can begin to form a plane through the graph that seperates good songs from bad songs. After a threshold has been found, the program can now compare any new songs it makes to songs that were considered "good" and determine if it has created a song that sounds good, if it determines it has created a bad song then it can restart its songwriting process and keep going until it produces a good song. It is important to note that although there are many algorithms available to find the threshold between good and bad results, they all essentially do the same thing so getting large amounts of data is the most important step in this process.

This resource answers the question 1: how can we implement machine learning?

### 2. How can we create an accompaniment?

One of the simplest accompaniments possible is a chord progression. By randomly selecting a key, or allowing the user to input a key of their choice, it is simple enough to create a progression of chords. According to [Chord Progressions], finding the euclidean distance between the attributes of two different chords results in variables that represent how similar the two chords are. These variables can then be converted into probabilities of substitution between chords and used to determine how likely it will be that one chord will follow another. I can use these probabilities to randomly generate a series of chord progressions that will serve as the accompaniment to the song.

This resource answers question 2: how can we create an accompaniment?

### 3. How can we create a melody?
The melody is the most complex part of the song to create, but it should prove to be fairly easy to create after breaking it down. The most important characteristic that determines whether a note will sound good in a certain position is its pitch, a note will sound out of place if it is drastically different than a note currently being played. All I have to do to solve this is determine what pitch should be played based off of the accompaniment, by picking only notes that harmonically agree with the chord currently being played in the accompaniment, I can be sure that there will never be a problem with harmony. 

According to [Music and AI], each event that occurrs in a song changes how the rest of the song is viewed. If there is a prolonged quiet note or silence for a while, then a sudden loud note will have a much greater affect on the audience. Likewise, a large amount of dissonance will cause the audience to feel a sense of anticipation as they wait for the cadence whereas consonance will not have nearly the same affect when it is not preceded by dissonance. To keep track of each of these, [Music and AI] proposes the idea of instantaneous probabilities which keep track of key characteristics of the song throughout the songwriting process. By keeping track of what has already been done, the song can check all the instantaneous probabilities each time a new note is to be written to give it attributes that will progress the melody.

This resource answers question 3: how can we create a melody?

[Machine Learning]: http://homes.cs.washington.edu/~pedrod/papers/cacm12.pdf
[Chord Progressions]: http://ismir2005.ismir.net/proceedings/1091.pdf
[Music and AI]: http://music.arts.uci.edu/dobrian/CD.music.ai.htm
