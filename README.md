Download Link: https://assignmentchef.com/product/solved-assignment-6-cmsc204
<br>
<p class="ui header product-top-header" title="Assignment 6 CMSC204 Solution">New concepts tested by this program

Implement Graph Interface

Use Graph to maintain a network of Actors

Shortest Path Algorithm implementation

Social networks are everywhere!  They connect people with other people.  There is an internet meme called “The Six Degrees of Kevin Bacon”, which describes how movie actors are connected, directly or indirectly, with Kevin Bacon.  Surprisingly, very short chains exist between any pair of actors, even obscure ones. For more information, see Six Degrees of Kevin Bacon and The Oracle of Kevin Bacon.

A Graph is a set of Vertices and a Set of Edges.  You will creating an ActorGraph that will be implementing a Graph interface with a set of Vertices of Actors and a set of Edges that identify the connection between two actors with a movie name.  The header for your ActorGraph will be as follows: public class ActorGraph implements Graph&lt;Actor, MovieEdge.

Within the Graph interface is a method dijkstraShortestPath.  You will be coding the Dijkstra’s Shortest Path algorithm.  You will then be able to find the connections between two actors through the movies that they have acted in.

For example, to connect Robin Williams to Charles Chaplin we might find:

Robin Williams via “Dead Poets Society” to Norman Lloyd

Norman Lloyd via “Limelight” to Charles Chaplin.

The ShortestPath algorithm typically uses a weighted graph which means that the edges have a weight, and this is used to determine the shortest path.  For this implementation, each weight will be 1, so that the shortest path is based on the number of movies in the path.

Data Element – Actor (Vertices)

You will be creating a class Actor which will hold all the information for an actor and implements Comparable.  For simplicity sake, we will store the name in a single String in the following format:  Last name, First name, so they can be sorted easily by last name.  For the JUnit test, you will need a constructor of the Actor class that takes in a string, which is the name of the actor in the format: Last name, First name.  You will also need a getName method to return the name of the actor in the format:  Last name, First name.  Follow the Javadoc for Actor.

Data Element – MovieEdge (Edges)

You will be creating a class MovieEdge which will hold all the information for an edge and implements Comparable.  It contains a source and a destination, both are Actor objects, a weight (use 1 for the movie shortest path), and a String which holds the movie name that these two actors are connected by.  It must have methods of getSource() and getDestination() which return the Actor objects and getMovieName() which returns a String with the movie name for the JUnit Tests.  Follow the Javadoc html for MovieEdge.

Data Structure – ActorGraph

You will be creating a class ActorGraph which implements GraphInterface.  The header for this class will be:  public class ActorGraph implements GraphInterface&lt;Actor, MovieEdge.  Implement the methods.  This is an undirected graph, which mean that an edge from Actor1 to Actor2 also means there is an edge created from Actor2 to Actor1.

Data Manager – ActorGraphManager

Implement the ActorGraphManagerInterface that holds an object of the ActorGraph data structure and has methods for maintaining the data structure. The ActorGraphManager takes input from the GUI and provides output to the GUI through methods such as addActor and addMovie.

GUI Driver

Create a GUI driver that will allow the user to read from a file to add Actors and Movies, or add Actors and Movies by typing in names.  It will then display the connections between Actors.  Use a FileChooser to allow the user to select a file to read from.

Beginning screen.  First read a file.

5/5 - (2 votes)