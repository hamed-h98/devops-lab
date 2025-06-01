# Microservices

### Source: https://www.youtube.com/watch?v=rv4LlmLmVWk


---

#### Monolith and its downsides

Before microservices, the standard way of developing applications was with a monolithic architecture. This means the whole code and all components was part of a single unit. 

For example if we have an online shop application, all of its parts like user authentication, shopping cart, product catelog, notifications, payment, etc, all code for all these functionalities would be in one code base as part of one monolethic application. 

Everything is developed, deployed and scaled as 1 unit. 

this means the application must be written in a single language with one technology stach with a single run time. 

If we have different teams working on different parts of the application, they will need to coordinate to make sure that they don't effect eachother's work. 

Also if developers change code for the payment functionality, you'll need to build the whole application and deploy it as one package. You can't just deploy only the payment functionality changes separately. 


<img src="images/image1.png" alt="Alt text" width="600">


























