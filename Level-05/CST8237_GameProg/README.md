# CST 8237 - Game Programming (2024 Fall)

## NOTE to STUDENTS!
- (Optional) If using `ZIP_DELIVERABLES`, make sure to MODIFY the following line (near the top):
`set "studentCode=abcd0000"`
... so that it matches your student email ID!

### Summary of scripts

- `CLEAN_SCRIPT`: This **deletes** all files & folders EXCEPT for the specified deliverables (ie. Config/, Content/, Source/, *.uproject).
  1. Prompts the user to Proceed, and
  2. Only runs `IF` the base folder contains "Lab" or "Assignment"
  3. Has a modifiable list of excludable items: a) folder names, and b) file extensions.

- `ZIP_DELIVERABLES`: This script is a much less destructive approach to selecting the files required for submission.
  1. checks whether **Unreal** (UE4, UE5, UnrealEditor) is **currently running** (it may still be using some files such as a Level) and tells the user to close the editor.
  2. checks whether any of the **required project folders** (from lists) and **.uproject** are **missing** and reports any missing items. 
  3. checks whether a ZIP archive (in the current folder) **already exists** by that name, and prompts the user to either **overwrite or cancel**.
