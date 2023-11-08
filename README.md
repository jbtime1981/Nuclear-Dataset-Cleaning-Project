# Nuclear-Dataset-Cleaning-Project
Excel files with original nuclear dataset, cleaned nuclear dataset, and a pivot table from the cleaned dataset.

Credit for original dataset below.
Utkarsh Singh.  "Nuclear Explosions Data" (2023 - Version 3). Kaggle. Retrieved August 2023.
https://www.kaggle.com/datasets/utkarshx27/nuclear-explosions-data

This project was predominantly an exercise in cleaning and exploring a dataset on the nuclear detonation records of seven countries from 1945 to 1996.

I used Google Sheets for the cleaning and analysis, and Tableau for the visualizations.  

For my cleaning process, I made a copy sheet of the original data in Google Sheets so that as I made edits I would still always have the complete, unedited dataset.  In the new sheet I froze and bolded column headers, standardized header names, and deleted rows with missing data.  I used this source (https://inis.iaea.org/collection/NCLCollectionStore/_Public/31/060/31060372.pdf) to update detonation type names for readability. I also deleted columns that were not useful (for example, data magnitude and yield columns), filtered out two countries that collectively only had five detonation observations in the dataset, leaving the top five most active countries; and finally removed detonation types that had five or fewer occurrences in the dataset.  

Now I was ready to start exploring the data.

I started by creating a pivot table to see how many of each detonation type had been conducted by each country.  I also included the totals of each country across detonation types, as well as the total number of detonations across all countries.

I created another pivot table, this time with the countries now categorized both based on detonation type and timeline.  This visualization shows when every country's detonations started and stopped (at least within this dataset).

A few trends stood out with this visualization.  The USA were the first to use a nuclear bomb in 1945.  The USSR soon followed in 1949.  These two countries were the first to begin using nuclear weapons and the most prolific.  The USA and France varied their detonation types the most.

Another noticeable trend was that certain detonation types seemed to stop being used before others.  The last Airdrop and Atmosphere detonation were done by China in 1976 and 1980 respectively.  Any at or above surface detonations seemed to happen less and less as time went on.

To explore this further, I decided to create a visualization in Tableau.  I combined detonation types and put them into three categories, Above, At, and Below the surface.  

The Above category included detonation types Airdrop, Atmosphere, Balloon, and Rocket.  The At category included Tower, Barge, Crater, Gallery, and Surface.  The Below category included Shaft, Shaft-Ground, Shaft-Lagoon, Tunnel, Underground, Underwater.

Once these categories were established, I downloaded from Google Sheets and then uploaded each .csv file (Above, At, and Below; and the cleaned dataset) to Tableau (see that viz here - https://public.tableau.com/app/profile/jordan.berry7904/viz/NuclearDetonationsOverTime-AboveAtandBelowEarthsSurface/AtAboveandBelow) to begin visualizing how detonation types had changed over time.

Tableau helped clearly show that the type of detonation did change with time.  Detonations above and at the surface experienced a sharp decline in the 1960s.  They had stopped entirely by 1980.
Detonations below the surface spiked in the 1960s, and continued into the early 1990s, with a few final detonations in the mid to late 1990s.
