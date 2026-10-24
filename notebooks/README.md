# notebooks

Numbered in run order. Clear outputs before every commit. One owner per notebook at a time. Every notebook opens with CONFIG, follows MAP, DO, SEE, CHECK, SUM, and carries interview angles where a technique is used.

| Notebook | Produces | Depends on | Teaches |
|---|---|---|---|
| 01_load_clean_booking | Merges the booking data and clean the booking data and creates one booking table | 06, 01 | 1,308,732 rows and dropped 2,442 rows where created_at was after slot_at (bad data) |
| 02_laod_clean_patients | Loads the patients data and cleans it  | 06, 01 | 303,153 distinct people and normalized phone + normalized name + DOB |
| 03_Analyse_data |   |  |  |
