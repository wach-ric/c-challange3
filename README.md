# Yelp-style Domain Code Challenge

This code challenge focuses on implementing a simplified Yelp-style domain using Python classes. The main entities in this domain are Customer, Restaurant, and Review, and the goal is to establish relationships and build functionality around these entities.
Getting Started

To set up the project, use the provided Pipfile to install the required dependencies. Ensure you have Python 3.10 installed on your system.

bash

pipenv install

Domain Entities
Customer

    __init__(given_name, family_name): Initializes a customer with a given name and family name.
    given_name(): Returns the customer's given name.
    family_name(): Returns the customer's family name.
    full_name(): Returns the full name of the customer.
    all(): Returns all customer instances.

Restaurant

    __init__(name): Initializes a restaurant with a name.
    name(): Returns the restaurant's name.
    all(): Returns all restaurant instances.
    reviews(): Returns a list of all reviews for that restaurant.
    customers(): Returns a unique list of all customers who have reviewed the restaurant.

Review

    __init__(customer, restaurant, rating): Initializes a review with a customer, restaurant, and rating.
    rating(): Returns the rating for a restaurant.
    all(): Returns all reviews.
    customer(): Returns the customer object for that review.
    restaurant(): Returns the restaurant object for that review.

Additional Methods
Customer

    num_reviews(): Returns the total number of reviews that a customer has authored.
    find_by_name(name): Class method - given a string of a full name, returns the first customer whose full name matches.
    find_all_by_given_name(name): Class method - given a string of a given name, returns a list containing all customers with that given name.
    add_review(restaurant, rating): Given a restaurant object and a star rating (as an integer), creates a new review and associates it with that customer and restaurant.

Restaurant

    average_star_rating(): Returns the average star rating for a restaurant based on its reviews.

Usage

python

# Example usage goes here

Notes

    Ensure you have drawn a diagram representing the domain relationships before starting the implementation.
    Prioritize writing methods that work over writing more methods that don't work.
    Test your code in the console as you write to ensure correctness.
    Refactor and adhere to best practices after getting the functionality working.