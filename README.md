# data-analysis

A playground for data analysis scripting.

## TODO

📋 Meals number column is off by one because it counts 0, need to make new column starting at 1<br>
📋 Clean up 0s from min meal size<br>
📋 New bin starts in the middle of a meal run, the meal will be counted in both bins

📋 Update the meal size calculation to use the file num as the bin boundaries<br>
📋 Currently in [Dev] FED PR Data Analysis under Experimental<br>
📋 Starts with def get_meal_timepoints(df, start_time):<br>
Meal Size = number of pellets within a unique meal, when meal is defined as pellets eaten within resets (when FR goes from high number back to 1)

Timestamp for the max FR completed: Generate new csv per file with the following two columns related to the times the FR changes from a number to 1: Date Time stamp of BP, FR number
Max FR is not Max FR completed but Max FR reached
Perhaps we should also calculate total left and total presses before reset?
Mean FR is incorrect calculation because it sums every FR value and divides it by all events, instead of only grabbing max completed FR→ will need to calculate from the other table
