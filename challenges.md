# Python Challenges

Used to learn and implement data structures and algorithms.

## Climbing Class

We will be creating a class that can simulate climbs and movements.

### Create a Hold class

First, we need to create holds. These are objects that are put onto the wall in order to create a climb. Holds have a few attributes associated with them. We need their width, height, and outward length. These are stored in centimeter values, rounded to the nearest integer. We also want to know what type of hold they are. Certain holds are used differently to others. Each hold can either be a: Sloper, Crimp, Jug, Jib. 

#### Intricacies

There are two holds, Crimp and Jib that have a size requirement imposed on them. Crimps must have an outward length of at most 2 centimeters. Jibs must have all of their attributes to be at most 2 centimeters. 

### Creating the Climb class

A climb is essentially a list of holds, each at a certain altitude. Create a climb class that stores a group of holds, each which have an altitude associated with them. The altitude is an integer which represents centimeters off the floor.

#### Setters and Getters

It will be useful to be able to put holds onto climbs and get the holds on a climb. Create functions to add a hold and the associated altitude to the climb, as well as a function that gets all the holds on the wall.

#### Altitude 

Now create a function that gets all the holds that are at a certain altitude on the wall. We also want to be able to get all the holds of a certain type (Crimp) and find all the altitudes at which these holds are placed.

#### Creating tests

Create at least 3 tests to ensure that your classes work as intended. You can use the unittest class --> https://docs.python.org/3/library/unittest.html.

### Completing a Climb

Climbs are completed when a climber can successfully reach the top of a climb. We are going to implement a simple method to check whether you can accomplish a climb when using the holds on a climb. Jugs allow you to reach up from the altitude it is at to an altitude that is at most 100 centimeters higher. Slopers give 60 centimeters of altitude. Crimps give 30 centimeters and Jibs give 20 centimeters. Create a function in the Climb class that checks whether or not a climb is able to be completed. 

#### Creating tests

Create at least 2 tests to ensure that your classes work as intended. You can use the unittest class --> https://docs.python.org/3/library/unittest.html.

### Extensions

Each hold now has a strength level associated with them. This means you need to certain amount of strength to be able to use that hold. Each climber has a reservoir of strength that they have available. Update Jugs to decrease strength level by a random amount between 1 and 3. Slopers are between 3 and 5. Crimps: 4 - 6. Jibs: 5 - 10. Now update the climb function to take in a total strength level and check if the climber was able to complete that climb with the strength level available. 



