# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given that a person keeps count of visitors
  in between server restarts

  When the server restarts

  Then manual visitor count kept by the person is added
  to the visit-counter

Scenario: Reconcile counts if the sensor is offline for a while

  Given that we know the exact time interval
  for which sensor went offline

  When the sensor is online

  Then reconcile it's count manually
