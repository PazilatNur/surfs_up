# Surfs_up Climate_change Analysis

## Overview:

In this analyis we look at Hawaii weather trends  in June and Decemer. We would like to identify the weather difference between these 2 months to define risk factors to a surfboard bussines. 


## Results:

1. Since June is during summer time, average and minimum temp is higher than Decemeber. 

2. Only 25% of the recorded temps in June is lower than 73, whereas 50% of the recoded temps during Dec is lower than 71. This indicate that during Dec at least half of the time, it would be colder. 

3. Compared to Dec, June temps changes are a lot smaller. The difference between min temp and median temp is smaller than what we observed in Dec. 


### Summar:

- This analysis shows that June weather doesn't fluctuate as much as in Dec. But I would also think that Dec temp is not too cold for a icecream businnes and possibly for the surf shop. 

- However, more data and analysis needed in order to make a better judment about all year round temps trends. As our next steps, we should look into precipitation by months and how much it rained and if it was raining on the previous or subsequent days as well.

Query exp:

- June precipitation: results = session.query(Measurement.date, Measurement.prcp).filter(func.strftime("%m" ,Measurement.date)=="06").all()

- Dec precipitation: results = session.query(Measurement.date, Measurement.prcp).filter(func.strftime("%m" ,Measurement.date)=="06").all()