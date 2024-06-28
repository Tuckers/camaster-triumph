## Improvements
This post processor works with Fusion 360 and the Camaster CNC at Triumph Workshop. I modified a couple critical areas to remove features that caused errors with WIN CNC and to dramatically improve safety by automatically adding "M5" - stop spindle and "G53 P1" - return to park commands at the end of operation.

## Usage
1. Import the post processor file into Fusion 360.

Select a toolpath and choose "Post process"

<img width="325" alt="Screenshot 2024-06-28 at 10 06 17 AM" src="https://github.com/Tuckers/camaster-triumph/assets/5509913/e8e98970-9846-4f83-8ae6-e5f06740adf9">

Choose import post processor button

<img width="1046" alt="Screenshot 2024-06-28 at 10 07 05 AM" src="https://github.com/Tuckers/camaster-triumph/assets/5509913/5efea62d-32f8-4d87-b6a6-3804e464f4be">

Select camster-triumph.cps file and open

<img width="912" alt="Screenshot 2024-06-28 at 10 07 12 AM" src="https://github.com/Tuckers/camaster-triumph/assets/5509913/44b5c0aa-49b0-4894-a65a-52ffca69f2ab">

2. During post processing ensure that you UNCHECK the "Use tool changer" option.
<img width="946" alt="Screenshot 2024-06-28 at 9 49 45 AM" src="https://github.com/Tuckers/camaster-triumph/assets/5509913/9ced0452-6ecb-4bfd-912e-9bc6649ccae8">
3. Always review your g-code file to ensure that M5 exists at the end of the file to ensure safe operation.
