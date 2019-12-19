# Knowledge tracing data fiddler
A python project that allows easy management of knowledge tracing data

 - Easy conversion between commonly used data format
 - Data cleaning 
   - Convert non-binary correctnesses into binary correctness
   - Remove (csv) rows where critical values are missing
 - Group non-grouped data by students to obtain attempt sequences per student
 - Filter data
   - By maximum attempt count (by splitting or cutting)
   - By minimum attempt count
 - Split into train and test set


 ### Attempts-skills-corrects (asc) format
 Contains student attempt sequences in row triples that contain:
 1. Number of attempts
 2. Skill ids of attempts
 3. Attempt correctnesses

Example contents for two students:
 ```
3
1,2,3
0,0,1
2
1,1
0,1
```
