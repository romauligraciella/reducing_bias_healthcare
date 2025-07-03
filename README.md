#  🏥  Bias Mitigation in Patient Satisfaction

## Project overview
This project investigates bias in patient satisfaction survey data from a local hospital. 
The analysis is conducted for a branch of the Ministry of Health, 
which aims to monitor and improve healthcare quality based on public feedback. 
Patients were asked to rate their satisfaction with the hospital's services on a scale from 1 to 10.
According to the Ministry’s guidelines, an average rating of 5 or below signals the need for deeper investigation and possible intervention.

## Initial Findings
From the raw dataset, the average satisfaction rating was: `Mean: 6.13`\
At first glance, this suggests that patients were generally satisfied with the hospital services. 
However, further inspection revealed potential biases and data quality issues, including:
- Unbalanced gender representation (e.g., more male respondents than female)
- Outliers, such as ratings above the valid range (1–10)
- Suspiciously high scores, possibly due to loyal patients or input errors\
![image](https://github.com/user-attachments/assets/8a3cf4c7-9810-4f9e-b1fa-aa487f992d25)

Given the Ministry’s goal of obtaining objective and reliable feedback, these issues needed to be addressed.

## Data Cleaning and Bias Reduction
To improve data reliability, I performed several preprocessing steps:
- Removed invalid entries (ratings outside 1–10)
- Eliminated outliers
- Balanced the gender distribution among respondents

After cleaning and rebalancing the data, the average satisfaction rating dropped significantly: `New Mean: 4.64`\
This updated result suggests dissatisfaction, which may have been masked in the original biased dataset.
![image](https://github.com/user-attachments/assets/b6d67d32-a5ad-4eed-9c03-101ac5d8b434)
  
## Additional Insight
I also explored how gender may influence satisfaction ratings:
| Gender | Average Satisfaction |
| ------ | -------------------- |
| Female | 2.78                 |
| Male   | 6.50                 |

This finding raises important questions:
Are female patients more critical due to heightened sensitivity to service quality?
Or are there systemic issues in how services are delivered to female patients?

## Conclusion
This project shows that removing bias can drastically change the interpretation of healthcare performance. 
A system that initially seemed satisfactory may, in reality, be underperforming for a significant portion of its patients.
Bias mitigation is essential not just for data integrity, but for ensuring equitable and responsive healthcare services.

# Recommendation
To uncover the root causes of dissatisfaction, Irecommend:
- Conducting focus group discussions with patients
- Gathering open-ended feedback
- Applying Sentiment Analysis and Topic Modeling on patient comments to detect themes contributing to low satisfaction
