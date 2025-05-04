# BookMyShow

This project simulates a ticketing platform like BookMyShow. For any given theatre, it displays:

Next 7 available dates

On selecting a date, all running shows along with timings are displayed



Part 1: Database Design

| Entity  | Attributes                                                             |
| ------- | ---------------------------------------------------------------------- |
| Movie   | movie\_id (PK), title, language, duration\_minutes, genre              |
| Theatre | theatre\_id (PK), name, location                                       |
| Screen  | screen\_id (PK), theatre\_id (FK), screen\_name                        |
| Show    | show\_id (PK), movie\_id (FK), screen\_id (FK), show\_date, show\_time |



Normalization
1NF: Atomic attributes, no repeating groups.
2NF: All non-PK attributes fully dependent on PK.
3NF: No transitive dependencies.
BCNF: All functional dependencies have candidate keys as determinant.



Part 2: Query
List all shows on a given date at a given theatre with timings
