# surfs_up
# Rice Coding Bootcamp Module 9 Challenge -Jupyter Notebook- -VS Code-
---

## Overview of the statistical analysis:

The purpose of the analysis is to analyze the Weather data of Oahu, Hawaii and extract the temperatures during specific months (June and December) over the course of years to determine if opening a Surf n' Shake could warrant investor backing, especially from  W. Avy. Weather was the downfall to his last surf shop investment so he is particularly interested in this data.

---
## Results:

Three key differences between June and December Temperatures

1 December has a notably lower minimum temperature than June
2 The mean temperature is slightly lower in December than in June, but difference seems neglegible
3 The Standard Deviation in December is greater than in June implying a higher variance in temperature

---
## Summary: ##

After using Pandas "describe" function to grab a short summary of the data, the similarity in mean temperature shows great promise that the investment into a surf shop in Oahu, Hawaii would be favorable. Especially given that the generally coldest month of the year in the northern hemisphere is December, the data taken from the past years shows that the weather is still in a good range for surfing. I believe W. Avy should invest in this endeavor.

### Additional Queries ###
---
* session.query(Measurement.date, Measurement.tobs, Measurement.prcp).filter(extract('month', Measurement.date) == 6)
* session.query(Measurement.date, Measurement.tobs, Measurement.prcp).filter(extract('month', Measurement.date) == 12)
---
Description: The above queries also grab precipitation data for the months of June and December. This data is worth the consideration as this can have an effect on whether people want to surf, eat icecream, or both!
