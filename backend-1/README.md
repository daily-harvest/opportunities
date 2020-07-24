# Introduction

Thank you for your interest in Daily Harvest! As the next step in our interview process, please complete the coding exercise below. This is a simplified instance  of the sort of functionality that we build for Daily Harvest customers. We may build off of your solution to this exercise in the on-site interview. Enjoy!

# Challenge

At Daily Harvest, we want to make it as easy as possible for our customers to get healthy food that they enjoy. One way to do this is to allow people to search   for products that contain a favorite ingredient (apples, kale, banana, coconut, etc.).

We have provided two files that define products and ingredients in JSON format:

[products.json](https://raw.githubusercontent.com/daily-harvest/opportunities/master/web-1/data/products.json) - the list of products
[ingredients.json](https://raw.githubusercontent.com/daily-harvest/opportunities/master/web-1/data/ingredients.json) - the list of ingredients

Daily Harvest uses python, so we'd like you to write a simple python program that returns all of the products that contain a requested ingredient.

Example: A search for the ingredient named “Organic Banana” should return the products named “Acai + Cherry”, “Chocolate + Blueberry”, “Cinnamon + Banana”, “Ginger + Greens”

Because we are an e-commerce company, we prefer that your solution be implemented as a REST API that we can validate using curl or Postman. If you prefer to submit a pure command-line solution, please construct it in a way that would allow the core logic to be exposed through a REST API without modification.

Good luck! We hope that you enjoy completing this challenge and look forward to seeing your approach to the problem.

# Requirements

* Please include a README that includes any instructions for configuring and running your program. Include any assumptions (version of python, operating system, etc.)
* Your solution should run without any modifications (code, file/directory structure, etc.) that are not specified in the README
* Your solution should accept the ingredient name (not id) as an input
* Your solution should return only products that contain the specified ingredient as output
* Your solution should handle reasonable error states and edge cases without throwing unhandled exceptions
* Your solution should provide useful output to the user for handled exceptions
* If you are applying for a senior or lead position, unit tests are required with your submission

# Notes

* Do not modify the JSON files.
* Keep your code as clean and readable as possible, utilizing idiomatic python style
