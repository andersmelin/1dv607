# Peer Review – Domain model, Jonathan Walken et al

We would like to start off stating that the domain model presented by this group analyzes the problem description as a whole, not only the requirements presented in the first iteration. That is, it includes requirements such as payment that was not included in the list of	[requirements](https://coursepress.lnu.se/kurs/objektorienterad-analys-och-design-med-uml/workshops-2/peer-review/) for this first hand-in. As such, the scope of the domain model is broader than expected, which should be kept in mind when reading this peer review.

The first impression of the domain model is that it is very visually appealing, owing to the care taken to color it in and give it a uniform look and design. This may not be a formal requirement of domain models as such, but part of thinking like a mapmaker – as Larman states,  *"make a domain model in the spirit of how a cartographer or mapmaker works"* **[1, p239]** is making sure that people will want to read your map, and the design goes a long way towards that.

On the other hand, as noted above, the domain model includes “irrelevant or out-of-scope features,” ****[1, p239]**** making the map cluttered and harder to read. Starting small, by including only the requirements as presented in this iteration, would have made the domain model slowly increase in size and complexity, which in turn would have made it easier to arrange the conceptual classes in a more fluid manner.

The biggest problem with the domain model, however, is the associations. While the group followed the naming convention perfectly, by starting with a capital letter and using hyphens between words, the names chosen for the associations could use work. One example is the association Treasurer Works-on Payment. This name is somewhat unclear, as we are unsure of how exactly the treasurer works on a payment. As Larman states, *“simple association names such as ‘Has’ or ‘Uses’ are usually poor, as they seldom enhance our understanding of the domain.”* **[1, p249]**. Perhaps a better name would be *"Processes*"", for example, depending on what work exactly the Treasurer performs on payments. We are aware that Larman uses the very same association in an example himself **[1, p254]** but that is referring to a cashier conceptual class who is doing his daily labor the conceptual class Register.


Another problem with the associations is that there are too many of them, when the guideline is to “be parsimonious about adding association lines” **[1, p247]**. Association lines such as *Membership Overview-of Payment* and *Secretary Schedules-event-for YachtClub* are not “need-to-remember” **[1, p247]** associations, and their presence restricts the flow of the domain model and adds visual clutter.

As for the conceptual classes identified, we believe that the group has included all the necessary, real-world conceptual classes for this iteration and given them adequate names. For example, the group has identified the need for a BoatInformation class in the domain model to solve the problems described by Larman in Chapter 9.13**[1, p234]**. However, again, there are conceptual classes identified that are not part of this iteration, so we cannot comment on those.
One observation for the conceptual classes is that some attributes have a type associated with them, such as dateTime: Date in the CalenderEventclass. This is a feature of design models rather than domain models, so we believe it should not be included.

**As a developer would the model help you and why/why not?**  
The model cointains all the necessary components to write a design model that fulfills the requirements so it would be helpful. The result would of course be a much bigger and complex model than actually needed, but it would indeed be helpful.

**What are the strong points of the model, what do you think is really good and why?**  
Very good use of attributes. Well thought out conceptual classes.

**Do you think a domain expert (for example the Secretary) would understand the model** We are sure that \*he would understand it. At firts it might seem confusing but given some time for analyzis \*he would understand it

**What are the weaknesses of the model, what do you think should be changed and why?**  
The weakest point is clearly that is is to broad including functionality that lies out of this scope. Solution would be to trim it to include only the necessary pieces

**Do you think the model has passed the grade 2 (passing grade) criteria?**  
Yes, the model has passed the grade 2 criteria, as it provides a usable domain model for a developer and for a domain expert, even with the requirements for future iterations included in the model.


Referances:
1. Larman C., Applying UML and Patterns 3rd Ed, 2005, https://aanimesh.files.wordpress.com/2013/09/applying-uml-and-patterns-3rd.pdf
