# **Project Reflection**

## What worked well 
Data acquisition was surprisingly seamless. The FRA's Blocked Crossing historical dataset is available to the public and simple to filter by date, city, state, even rail company. Additionally, the webpage has several graphs and infographics to easily make sense of the data visually. The ease of exporting an .xlsx file with filtered settings, made the task of data preprocessing and cleaning easier.

Data preprocessing and cleaning worked as intended. The dataset naturally has missing fields as it is collected from public reports of rail blockages. This was handled by simply removing irrelevant columns (like `Time_Window` and `Additional Comments`), removing duplicate reports, and filling in missing fields with standardized data ie. missing fields in `County` are filled in with `Harris`. Reducing the dataset to focus on Union Pacific reports only (98.3% of the original dataset) further simplified the overall process. The final cleaned dataset contained 16,864 records after starting with 20,783 records.

Training the GRU classifier exceeded expectations: the model performed at an 85% accuracy on crowd-sourced, real-world data. Lowering the threshold from 0.50 to 0.40 improved recall from 84.9% to 89.7%, which shows that the agent now catches nearly 90% of high risk events. The demos showed that the agent had actually learned real patterns, when Leeland Street at rush hour returned a 93% HIGH vs 6% overnight risk, reflecting real trends.

The addition of a street name lookup tool made the agent much more user friendly. At first the agent's output was only displaying the Crossing IDs, a series of numbers and letters, for example "411912V". After adding the tool, the output displayed the actual street name, which would be more practical in a real-world scenario.
## What did not work and how it was handled

## Biggest technical challenged and how it was solved

## Path changes from the Midterm blueprint

## Next plan of action 
