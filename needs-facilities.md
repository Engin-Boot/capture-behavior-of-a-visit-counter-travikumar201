# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given that there is a sensor at the entry door and it
  increments by one when someone enters

  When the visitor count for each day is recorded accurately

  Then visitor trend for the week is calculated

Scenario: Alert when seating capacity is full

  Given that there is a sensor at the entry door that counts number of people

  When the count from sensor equals to the seating capacity of the room
  
  Then accommodate the visitors in another room
