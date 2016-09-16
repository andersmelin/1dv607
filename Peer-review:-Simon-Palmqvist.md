# Peer Review – Domain model, Simon Palmqvist

The model presented by Simon has few (five) conceptual classes, which is good because it keeps the domain model small and very easy to read, removing clutter from the domain model. Larman states that a good domain model should not include superfluous conceptual classes [quotation needed]. The amount of information required for the problem description in this first iteration is not very high, which means that a small domain model is perfect for it. This also leads to the domain model being arranged very neatly, further improving readability. However, we believe that the problem description required conceptual classes that Simon has not included in his model, which despite the advantages of keeping the number of conceptual classes down makes it somewhat incomplete.

The two conceptual classes we identified that are lacking in this domain model are Calendar and Secretary. Although Simon notes that he considered including the Secretary class but then removed it, we believe that this class is required on a "need-to-remember" [citation needed] basis, as this class models the person that is responsible for managing and assigning berths. We also believe the Calendar class is necessary, but Simon may disagree on this point.

Moving on to the associations of the model, we have a few points to consider. First, the association Member Attends Event is out of the domain scope, as the problem description only mentioned viewing and listing events, not attending them. As Larman states, “irrelevant or out-of-scope features" [citation needed] should be avoided. Another thing to note is that the multiplicity of the association Boat Docks-at Berth, or 1 - 1, should be 0, 1 - 1, to show that berths can (and often are) empty. Another option is 0, 1 - 0, 1, as boats can exist in the system without being assigned to a berth, for example in wintertime when they are kept on land.

**As a developer would the model help you and why/why not?**  

Yes, because it contains an adequate number of classes and associations to begin working on a design model for this iteration.

**Do you think a domain expert (for example the Secretary) would understand the model why/why not?**  

Yes, the classes and associations have good, real-world names and the simplicity makes it easy for a domain expert to follow. Of course, the Secretary would probably want to be included in it.

**What are the strong points of the model, what do you think is really good and why?**  

The strong parts, as we described above, are the arrangement and simplicty of the domain model. Simon has clearly worked "in the spirit of how a cartographer or mapmaker works" [citation needed] and has created a good, readable map from the outlined requirements.

**What are the weaknesses of the model, what do you think should be changed and why?**  

We have described the weaknesses we found above: namely, some issues with conceptual classes we believe should be included and some problems with the associations between conceptual classes.

**Do you think the model has passed the grade 2 (passing grade) criteria?**  

The issues we found are relatively small and so overall, we feel that the domain model has certainly passed the grade 2 criteria.
