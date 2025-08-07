# CS101-finalProject-Udacity gamers network

# Gaming Social Network - CS 101 Final Project

## Overview
This project implements a gaming social network where users have connections (friends) and games they like to play. The program parses a block of text input to create a network and supports various operations, including adding new users, making connections, finding common and secondary connections, and finding paths between users. The network is represented using a dictionary, with each user having their own list of connections and games.

## Key Features
- **`create_data_structure`**: Parses input to create the network.
- **`get_connections`**: Returns a user's connections.
- **`get_games_liked`**: Returns a user's liked games.
- **`add_connection`**: Adds a connection between two users.
- **`add_new_user`**: Adds a new user with game preferences.
- **`get_secondary_connections`**: Finds secondary connections.
- **`count_common_connections`**: Counts common connections between two users.
- **`find_path_to_friend`**: Finds a path between two users using recursion.

## Example Usage
```python
# Initialize network from example input
network = create_data_structure(example_input)

# Get connections of a user
print(get_connections(network, "John"))

# Get games liked by a user
print(get_games_liked(network, "John"))

# Add a connection between two users
network = add_connection(network, "John", "Freda")

# Add a new user to the network
network = add_new_user(network, "Nick", ["Seven Schemers", "The Movie: The Game"])

# Get secondary connections of a user
print(get_secondary_connections(network, "Mercedes"))

# Count common connections between two users
print(count_common_connections(network, "Mercedes", "John"))

# Find a path from one user to another
print(find_path_to_friend(network, "John", "Ollie"))

