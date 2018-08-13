
# Codaisseur final indivual assingment
For our final evaluation we had to create an event ticket marketplace, combined with an Uber pickup service. We needed to implement authentication and authorization. An important part of the assingment was to come up with a fraud algoritm that calculates the risk of a ticket that is for sale on the platform. 4 days of hard work and little sleep, but in the end I am happy with what I was able to build in this short amount of time.

A live version of the app: https://enigmatic-beyond-14205.herokuapp.com/

# Technologies used
Frontend:
-React
-Redux
-Redux thunk
-React router
-Superagent
-Material UI
-Styled Components

TypeScript backend:
-Koa
-TypeORM
-Postgres
-Routing controllers
-Class validator
-Json webtoken


# Learnings
I am not happy with the code in the event.js reducer. Because I had to deal with nested data the code is not very clean. Next time in a situation like this i would use Normalizr to normalize the data that is coming from an API.
I also had a situation where I made a POST to the server and changed the route at the same time. Because of the asynchronous nature of the server call, the chaning of the route went faster than the response from the api, and this gave me some unwanted effects. Because of time restraints I changed the route after a setTimeout, wich is probably not a good practice. A codaisseur teacher gave me the tip to use react-router-redux to handle route changes in async situations.      

