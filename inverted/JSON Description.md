# Description of the JSON File Structure:
*now inverted*

1. **Division**: The name of the division (i.e. Product and Engineering, Marketing...)
2. **Days**: The days (at least 5 and up to 7) that are captured from the last week to indicate performance
    1. Each day records the following information:
        1. **Date**: The actual date.
        2. **Overall Score**: The execution score of the division, indicated by the line graph on the top right hand corner in the SQOR Dashboard.
        3. **Performance**:
            1. An array containing the execution score (labelled: *score*) of a given tool for the past five days. In the future, the execution score will be replaced with the KPIs for each tool and its reported usage for that day.
                1. **Tool Name**: The name of the used tool in the division
                2. **Status**: The status of the given tool (whether it is active listing scores or inactive meaning recognized by the dashboard but not being tracked)
                3. **Score**: The execution score for the tool on the given day.
                4. **Percent Change**: The percent increase/decrease of the execution score of the tool compared to the previous day.