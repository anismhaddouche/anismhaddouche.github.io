---
layout: page
title: Collaborative Writing
description: Measuring Collaborative Writing with NLP
img: assets/img/IMT.png
importance: 1
category: work
---

## Project summary
Collaborative Writing (CW) is a common activity in education, which is being enhanced by the use of digital learning environments, leading to a growing research field in Computer-Supported Collaborative Learning (CSCL). 

In order to help teachers to monitor students CW, we developed in this projet  two indicators that provide measures of student contributions to a text writing, namely balance of contribution and co-writing. We also identified CW strategies that are well defined in the literature.

Moreover, we conducted a questionnaire evaluation to verify the interpretation of the indicators and the strategies by teachers in higher education context, using student reports edited in a collaborative digital environment called [LabNbook](www.labnbook.com), during physics and chemistry courses in undergraduate level. Results showed that teachers have a good interpretation of the indicators and strategies. This work contributes to research insights in CW, and motivates future work to design meaningful learning indicators.


## Technical Implementation

The **balance of contribution** and **co-writing** indicators were implemented using Python to process and analyze collaborative writing data. These indicators provide detailed insights into the contributions of each student within a collaborative digital environment.


The **balance of contribution** indicator measures the proportion of text contributed by each student in a collaborative writing activity. To calculate this, we:
- Extracted the version history of the text.
- Tracked the number of words and edits made by each student.
- Normalized these values to compute each student's relative contribution.

The Python implementation uses libraries such as `pandas` for data manipulation and `numpy` for numerical operations. Here is the link to the code for this indicator:
[GitHub - Balance of Contribution Implementation](https://github.com/yourusername/your-repo/balance-of-contribution.py)


The **co-writing** indicator focuses on identifying moments when students actively worked together on the same section of the document. The approach includes:
- Analyzing time intervals of text edits.
- Detecting overlapping edits made by different students.
- Calculating the degree of simultaneous contribution.

This part of the implementation uses time series analysis and relies on libraries such as `matplotlib` for visualizing edit patterns. The code for the co-writing indicator can be found here:
[GitHub - Co-writing Indicator Implementation](https://github.com/yourusername/your-repo/co-writing-indicator.py)

### Tools and Libraries Used

- **pandas**: For data handling and processing.
- **numpy**: For numerical computations.
- **matplotlib**: For visualizing contribution timelines and co-editing events.
- **GitHub API** (optional): For accessing and analyzing real-time collaboration data from repositories.

You can find the full source code and documentation in the GitHub repository:  
[GitHub - Collaborative Writing Indicators Project](https://github.com/yourusername/your-repo)

### Next Steps
The next phase involves optimizing the computation of these indicators for real-time analysis and integrating them into the [LabNbook](https://www.labnbook.com) platform.
