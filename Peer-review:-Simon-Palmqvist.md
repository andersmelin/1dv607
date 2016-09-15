# Peer Review – Domain model, Simon Palmqvist

## Francis, Consider:

**Basically** it's a very good model, here is what I could scrap together to be considered misstakes

```
Member <---[Attends]---> Event
Out of scope! Member <---[Views]---> Event - but whether or not he attends is not part of the model
```

```
Boat [1] <------> [1] Berth
SHOULD BE:
Boat [0,1] <------> [1] Berth (Berth might have no boat)
OR
Boat [0,1] <------> [0,1] Berth (Waiting to be assigned/ wintertime on land)
```
```
MISSING CONCEPTUAL CLASSES:
Calendar and Secretary. We see them as necessary to fulfill the requirements (that is: assign Berth and add Event).
```

## Headlines below

**As a developer would the model help you and why/why not?**

**Do you think a domain expert (for example the Secretary) would understand the model why/why not?**

**What are the strong points of the model, what do you think is really good and why?**

**What are the weaknesses of the model, what do you think should be changed and why?**

**Do you think the model has passed the grade 2 (passing grade) criteria?**
