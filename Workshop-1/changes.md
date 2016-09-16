# Changes to our model

We decided to follow the advices we received in the peer reviews as follows:

- Added an arrow marker from *Secretary* to *CalendarEvent* since the flow goes opposite the default direction
- Reduced an association between *Member* and *CalendarEvent*. One association is enough (if using 1..\* instead of 1 as multiplier). Did it to reduce clutter.
- Reduced associations between *Member* and *Boat*. Reduced noise by only using one connection
