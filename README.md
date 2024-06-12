## Knapsack Decision Task used for fMRI study

The task is coded using Unity Game Engine with C#. 

Here, you will find the standard Unity project folder structure. The project can be used to build the task using Unity. The fully built task is not provided in this repository due to storage space concerns. 

Input/Output data folders are located in Assets/DATAinf. This folder has to be added manually to the game after building.

### Task description

In this task, participants are asked to solve multiple instances of the (0-1) knapsack decision problem (Fig~\ref{fig_task}a). Each trial presents them with a set of items, each with distinct values and weights, along with a capacity constraint and a target profit. The participant's task is to determine whether a subset of these items exists such that (1) the cumulative weight is less than or equal to the capacity constraint and (2) the total value meets or exceeds the target profit.

Each trial comprises four stages. Initially, in the items stage lasting 3 seconds, only the items are displayed. The value of each item, in dollars, is represented by dollar bills, and the weight, in grams, is shown within a black weight symbol. The size of the dollar bill increases with the item's value, and similarly, the size of the weight symbol increases with the item's weight. A green circle in the center of the screen indicates the remaining time in this stage. Next, in the 22-second solving stage, the target profit and capacity constraint are added to the screen within the green timer circle. During the 2-second response stage, participants see a YES' and a NO' button on the screen, along with the timer circle, and they respond using the keyboard (Fig~\ref{fig_task}a). Finally, a variable inter-trial rest period of 8, 10, or 12 seconds is displayed before the start of the next trial.

The task consists of 56 trials (7 blocks of 8 trials), each presenting a different instance of the knapsack decision problem. The sequence of instances is determined for each participant independently based on the `Assets/DATAinf/Input/KPInstances/XX_param2.txt` files. Where XX represents the participant's randomization number. The placement of the 'YES' and 'NO' buttons is also randomized between the left and right positions.

![exp_design](https://github.com/jpfranco123/KS-Decision-T2/assets/26372744/77f7302c-9658-4f01-8a5c-a52c91131459)

### Game controls:
- At the start of every block, the space bar has to be pressed for the game to proceed to the fixation point screen.
- Fixation point screen is presented at the beginning of each block until a ’T’ (scanner trigger code) is received.
- Buttons for the left and right answer buttons (YES/NO or NO/YES) are ‘b’ and ‘c’, respectively.

**Note:**
The key screen differences with the task used for the previous behavioral study are:
- Bill luminance was changed, and
- Weights were changed from ‘kg’ to ‘g’.
