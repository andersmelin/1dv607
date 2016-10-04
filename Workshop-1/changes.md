# Changes to our model

We decided to follow the advices we received in the peer reviews as follows:

- Added an arrow marker from *Secretary* to *CalendarEvent* since the flow goes opposite the default direction
- Reduced an association between *Member* and *CalendarEvent*. One association is enough (if using 1..\* instead of 1 as multiplier). Did it to reduce clutter.
- Reduced connections between *Member* and *Boat*. Less noise by only using one connection

After grade fixes by our teacher, we implemented the following change:

- Removed link between *Boat* and *Berth*
- Created new entity, *BoatAssignment*, with connections to *Boat* and *Berth*
