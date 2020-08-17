# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given that the hospital is open for patients

  When a new patient registers for diagnosis or treatment

  Then add one to number of patients that visited the hospital

Scenario: Compute parking slots to reserve for visiting specialists

  Given that a specialist is expected to visit the hospital on a particular day

  When the doctor approves his visit

  Then I add one to the number of parking slots to be reserved
