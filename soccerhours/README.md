Project Soccer Hours

This initial phase in App building will only involve data modeling, database definitions and the requisite functions in Python.

A list of the functions :

1. Add a new user (admin only)
2. Add a new venue (admin only)
3. Start an event (user or admin on behalf of a user)
4. Display timeslot availability at a venue
5. Display all venues where a particular timeslot is available
6. List events at a venue given date/time
7. User joins an event
8. Remove an event (admin only)


Assumptions:
1. Slots available from 8AM to 8PM as Start times for all venues
2. 1 hour Slots
3. User who creates, automatically joins event
4. All future slots for given dates are available unless event is booked on that slot
5. Event is active even if capacity is not filled
6. On Function 5,6: We show all overlapping events within the given timeframe(start+end)
7. Soft delete of events.

Convention:
1. User IDs start with 101
2. Venue IDs with 201
3. Event IDs with 301
4. Start and End times taken as Hours on 24-hour clock format
5. Named slots in ascending order : 8-9 is 1, 9-10 is 2
