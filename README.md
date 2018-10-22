# Functionality
## Basic functionality:
- Users who can login / logout
- Users will input their paramaters for type of activities they like,  and will be given a short list of different types of suggestions.
    - types of activities include:   
    - TV shows to watch
    - movies to stream.
    - movies to see in person.
    - restaurants to go to / try
    - Events happening nearby to go to.
- Users will have the option of being connected with other users doing the same activity, or of staying anonymous

## Optional add on functionality.
- users have the ability to friend other users
- users have ability to make lists of events and activities to save for later use
- suggestion algorithim learns over time based on users inputs.  

# Outline of tasks to accomplish
## User Auth
- Users can sign up, log in, log out
- DB stores user infomation
  - DB stores all of a users info, as well as their preferences:
    - user info: Name, email, DOB, gender
    - user preferences: TV / movie preferences (to be specified later), Restaurant preferences, Activity preferences, budget (in number of dollar signs), amount of time they wish to spend, how active they want to be.
- all of this has to be changable from the front end

## Make streaming recommendation
 - Use user's subscriptions to filter possible movies / TV from APIs from streaming services.
 - Use APIs for popular TV / movies trending
 - Algorithm uses user preferences to randomly select from the top X from TV and movies, accounting for user preferences

##  Make theatre recommendation
   - Use APIs for popular new movies to find films,
   - Use APIs for movie theatres with showtimes
   - Cross reference to user preferences in movies and use algorithm to make recommendation from the top X, accounting for current time and time of movie.

## Make restaurant recommendation
  - Use APIs for popular new or successful restaurants
  - if possible, integrate open table API for embedded ability to make reservation
  - accounts for restaurant preferences and budget
  - possible functionality of choosing this contingent on connecting with a user to go with.

## Make event recommendation
  - Use APIs for local events happening that day
  - Filter for things related to user's interests / budget
  - Use Algorithm for suggestion based on distance / price compared to budget

## Connect Users function
  - Upon selection of an event, users have an option of being connected or staying anonymous
  - If selection connected, they are connected with other users doing the same thing.
    - if selection a streaming option, connected with users anywhere doing the same thing
    - if selecting a physical activity, connected with other users doing the same thing at same location
  - either chat / message functionality for connected users

# Possible jobs for people in the group

- Front End 1  (Chris)
  - Designs the visual look of the site and the user interface and user experience to make it an appealing app.
  - Implements front end and collects data from from users about preferences.
- Front End 2 (Stefanie)
  - Assists in implementing all front end features.
  - Makes front end interface with all API calls  / backend data.
- backend / dataflow manager (Joe)
  - in charge of organazing the format of data from place to place so everything is on the same page
- manager for all API interfaces  (Tony)
  - collects all APIs needed, and finds correct ways of interfacing with them to gather all requisit data
