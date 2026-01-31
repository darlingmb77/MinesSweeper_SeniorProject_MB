# MinesSweeper_SeniorProject_MB
My interpretation of that classic Windows game

Project Proposal: Strategy-Based Minesweeper Web Application
###**Introduction**
Given that this is my last year of college, I chose to proceed with the more exciting and fun coding application for this project.  I plan to create a Minesweeper web-based application that combines game logic, data persistence, and performance analysis for users. The purpose of this project is to develop a fun, interactive game that I get to work on throughout the semester by following the phases of the software development life cycle. By the end of this project, I should be able to implement tests and refine the project to become something I can be proud of for my college career, showcasing all that I have learned from Santa Fe College.
###**Purpose of Software**
The purpose of this game is to recreate in a new modern way the Minesweeper that was a mini people's favorite Windows desktop game application. This project will offer the user a dashboard to view past statistics on games played by other users. This will be done with front-end development, back-end API design, database, and client-server communication. Fully encompassing an educational and strategy-based fun project.
###**High-Level Functional Requirements **
At the high-functioning level, the application will allow users to play the mind sweeper game through the web interface that will be built with React. The users will be able to start and interact with the game board pieces to complete the different games.  When a user starts a game, they will be prompted for a username. The application will send the user's completion score, username, and completion time through the REST API hosted on Render to my SQL database.
###**Survey of Relevant Tools and Literature**
Several technologies and learning resources will support the development of this project, such as React documentation and tutorials from YouTube from helpful programmers, and MySQL documentation. With Node.js and Express.js offering patterns for RESTful APIs, MySQL provides documentation for different database SQL designs and querying. Hosting platforms such as Render have several practical examples of cloud-based API using these different materials and tutorials related to the web-based game. The overall design approach will be covered by helpful resources.
###**Similar Software and Comparison**
Several different versions of Minesweeper already exist for web-based Minesweeper. Using those tools and the literature provided from minesweepers on Wikipedia about the description of how the game works will offer knowledge on assessing applications similar to those that I will be developing.  Understanding that this project differs by focusing more on the simplicity and custom analytics rather than the commercial gaming features that come with the others, not to mention the fact that this project will be made from the ground up, will solidify the uniqueness of this version of the gaming application.
###**Input, Processing, and Output **
Input will be done clearly by the user with the interactions on the board, including mouse clicks, game selection, and flag placements. Additional user input will be the username to tally the score as you would at an arcade game, not requiring users to input a password or account information. Processing will be developed to be on both the server and client sides. On the front-end, HTML will handle game logic with tiles and check winning conditions, for example, and the back-end API processes the request and validates data while managing the database interactions. Output of the system includes the game state, the end-of-game results, and a statistical dashboard, showing win rates, top winners, displayed with times, and by points.
  -•	Display a statistics dashboard showing:
    -o	Past game performance
    -o	Win/loss ratios
    -o	Best completion times
  -•	Compare player performance through leaderboards
  -•	Allow users to track improvement over time
**Data Storage and Data Sources**
The application will have its database storage and data sources from a MySQL database, which is an external application. This includes the tables for users, a collection of individual games played, and aggregated results. The data will be generated internally by the application itself without the use of third-party external API's and web scraping. Using Node.js app to Render for basic connections between repo and live app integrations. Stored data could be used to generate dashboards and show the comparison of top players based on time and correctly guessed tiles.
  -•	Data is generated internally by the application
  -•	User input collected through:
    -o	Game interactions (mouse clicks, flag placements, tile selections)
    -o	Username entry at the start of each game
  -•	Game results are sent from the React front end to a backend REST API
  -•	The API stores all data in a MySQL database
  -•	User-entered usernames (no passwords or personal account information)
  -•	Individual game records, including:
    -o	Game completion time
    -o	Game outcome (win or loss)
    -o	Score or points earned
    -o	Number of correctly guessed tiles
  -•	Aggregated game statistics, such as:
    -o	Win rates
    -o	Top completion times
    -o	Leaderboard rankings
    -o	Overall performance trends across users
**Project Plan and Conclusion**
In conclusion, this Minesweeper strategy-based application project will start with the different requirements needed for the definition and system design, followed by development of the front-end game, logic, back-end API, and database schema. Using all the criteria in this proposed project specifications, this application will be able to integrate with databases, RESTful API, and interactive interfaces offered to users with a strong foundation for helping me improve and learn while practicing real-life system designs from the ground up.


##**Example User Stories**
1.	As a player, I want to enter a username before starting a game so that my score can be saved and compared with others.
2.	As a player, I want to click and flag tiles on the game board so that I can play Minesweeper using familiar rules.
3.	As a player, I want to see my completion time when the game ends so that I can track my performance.
4.	As a player, I want to view a leaderboard so that I can compare my results with other players.
5.	As a player, I want to see past game statistics so that I can analyze strategies and improve over time.

##**USE CASES**
###Title: User Case 1 - Start a New Game
System: Minesweeper Web Application Front End
Actor: Player
Precondition: The application is loaded in the browser
Scenario:
•	The player enters a username.
•	The player selects a new game.
•	The system initializes the game board and timer.

Expected result: A new game will begin.


###Title: User Case 2 - Interact with Game Board
System: Minesweeper Web Application Front End
Actor: Player
Precondition: A game is active
Scenario:
1.	The player clicks tiles to reveal them.
2.	The player flags suspected mines.
3.	The system updates the board state accordingly.
Expected result: The game progresses toward a win or loss.


###Title: User Case 3 - Complete a Game
System: Minesweeper Web Application Front End
Actor: Player
Precondition: A game is in progress
Scenario:
1.	The player successfully clears the board or triggers a mine.
2.	The system stops the timer.
3.	The system calculates the final score.
Expected result: Game results are generated.

###Title: User Case 4 - Save Game Results
System: Backend API and Database
Actor: Player
Precondition: Game has ended
Scenario:
1.	The system sends game data to the REST API.
2.	The API validates the data.
3.	The data is stored in the MySQL database
Expected result: Game results are saved successfully.

###Title: User Case 5 - View Statistics Dashboard
System: Minesweeper Web Application Front End
Actor: Player
Precondition: Stored game data exists
Scenario:
1.	The player navigates to the statistics dashboard.
2.	The system retrieves aggregated data from the database.
3.	The system displays leaderboards and statistics.
Expected result: Player views performance analytics.
