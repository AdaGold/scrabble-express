# Exercise: Express Scrabble
The goal of this exercise is to practice with RESTful routing as expressed by a Node Express application. We will utilize our Scrabble code from the previous project to create a website that can score Scrabble words for us.

## Requirements
- Implement a home page (`GET /`) that has at least one (preferably cute) image and a navigation that links to the static `GET` routes below.
- Implement a route file and controller file for a ScrabbleController that responds to these routes:
  - `GET /scrabble/chart`: shows the letter score chart
  - `GET /scrabble/score`: shows a form allowing a user to submit a word for scoring
  - `POST /scrabble/score`: processes the user input and renders either
    - a page showing the user submitted word and it's score __or__
    - in the case of something it can't score, an error page with an "unscorable word" message
- `GET /scrabble/score/:name`: A dynamic route that scores whatever word is passed into the `:name` portion of the dynamic route. Will render either
  - a page showing the user submitted word and it's score __or__
  - in the case of something it can't score, an error page with an "unscorable word" message
