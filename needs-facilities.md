# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given that there is a sensor at the entry door that counts number of people

  When a new visitor arrives, the count of sensor increases by one
  
  Then I can keep a count of daily vistors for the whole week

Scenario: Alert when seating capacity is full

  Given that there is a sensor at the entry door that counts number of people

  When the count from sensor equals to the seating capacity of the room
  
  Then I need to open up another room to accomodate the visitors
