# usa-guess-game-in-python
A visual guessing game with pandas and turtle
First, the necessary modules turtle and pandas are imported.

A turtle screen object is created, with the title "U.S States Game" and a custom image of a blank U.S. states map is added as the background image.

The data of all 50 states in the U.S. is loaded from a CSV file called "50_states.csv" into a pandas DataFrame.

A list called all_states is created with the names of all 50 states in the DataFrame.

An empty list called guessed_state is also created to store the states that the user correctly guesses.

A while loop is used to repeatedly prompt the user to enter a state name until they have correctly guessed all 50 states or they enter "Exit".

If the user enters "Exit", a list called missing_states is created with the names of the states that the user did not guess correctly, and a new DataFrame is created from that list and saved to a CSV file called "states_to_learn1". Then the loop is broken.

If the user enters a state name that is in the DataFrame, the name of that state is added to the guessed_state list, and a turtle object is created at the location of that state on the map. The turtle then writes the name of the state on the map using the write() method.
