---
name: Learning Management System and Student Privacy Research [2023]
tools: [Research, mix methods, privacy, LMS, student data, policy]
image: 
description: What do we know about the learning management system user data collection?
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

# Privacy concerns among university students towards Learning Management System Data Collection

###### This project is a part of IS304: Advanced Research Design


### Abstract

After the spread of COVID-19 pandemic in 2020, universities adjust their services in order to provide students to4 continue their studies virtually. One approach is to have a learning management system with courses available for students. In this project, we identify the data collected by the learning management system that third party vendors have access to as the challenge to online learning as well as its influence on students’ concerns after the acknowledgement. We investigate each learning management that is currently at University of Illinois at Urbana-Champaign to create the list of data being collected and gather the information from the university students by using surveys to reflect their concerns. The outcomes present the individual feeling indifferent despite learning new information from the privacy policy.

### Methods

In order to gain an understanding of the student perspective, mixed methods are used to explore and analyze the findings. The first step is to collect privacy policies collected by the LMS that the University of Illinois at Urbana-Champaign used to operate or is currently using as well as the list of the third-party vendors that have accessed the LMS user data. I conduct a qualitative analysis of each LMS privacy policy to extract the information and put one or two excerpts from each LMS in the survey that will be responded to by the University of Illinois at Urbana-Champaign students. After that, I create the survey that contains the preliminary question followed by the excerpts and/or list of third-party vendors for each LMS along with the questions that ask them to respond by reflecting on the information they learned. Some of the preliminary questions are about the respondents' majors, class standing, and familiarity with privacy. The second parts of the questionnaire, for example, are whether they think the excerpt about the third party is reasonable, and whether acknowledgment of the earning management system privacy policy affects their concerns or not.
  
After the process of data collection, I will use the Python programming language to do the data cleaning, and descriptive analytics, and analyze the survey results. Data cleaning includes deleting the personal identification of the participants and converting the dataset to a new format that is ready for analysis. Descriptive analytics will be used to show the general information about the participants such as the bar plots containing the frequency of each class standing or colleges they are in, and the word cloud showing all the majors participating in this survey. Finally, we will use the correlation coefficient and content analysis to identify the patterns that emerged from the dataset. The correlation matrix will be created based on the interests of at least two variables or questions from the survey. The content analysis will be used to segment the participants into groups according to their overall responses to the survey.

### Results
The results show significant decreases in reading privacy policy in the learning management system compared to the normal website which shows that individuals tend to trust the academic software more than the non-academic platform. After learning about the Canvas privacy policy, approximately 70 percent of the participants feel neutral and not concerned about their privacy. For respondents who feel neutral shows a strong relationship with their concerns before and after their acknowledgment. 
  
Based on the final results, we learned that the majority of the respondents do not concern or take an interest in privacy even though they are a part of data collection. Despite the outcomes, new information is learned by the participants which indicates the lack of transparency or informed consent to the users, in this case university students. Therefore, the current policy approach might be as effective in transparency. One alternative approach that could be used to improve the transparency of the learning management system is by providing the privacy label that looks like a pop-up that contains the concise summary of the information being collected and how it could be shared to the third party vendors. Doing so will reduce the responsibilities from users perspective to read the whole documents of the learning management system privacy policy. The user can have a glimpse of what is being collected by understanding the privacy label that could take at most a minute of reading.


### References

Apps Run The World, & Statista. (December 22, 2021). Size of the education software/application market worldwide from 2019 to 2025 (in million U.S. dollars) [Graph]. In Statista. Retrieved February 22, 2023, from https://www-statista-com.proxy2.library.illinois.edu/statistics/643909/worldwide-education-software-market-size/?locale=en

Jones, K. M. (2019). Learning analytics and higher education: a proposed model for establishing informed consent mechanisms to promote student privacy and autonomy. International Journal of Educational Technology in Higher Education, 16(1), 1-22.

NCES. (December 31, 2021). Number of postsecondary students enrolled in distance education courses in the United States in fall 2020 (in 1,000s) [Graph]. In Statista. Retrieved February 21, 2023, from https://www-statista-com.proxy2.library.illinois.edu/statistics/987887/number-college-students-enrolled-distance-education-courses/

U.S. Department of Education. (2021, August 25). Family Educational Rights and Privacy Act (FERPA) [Guides]. US Department of Education (ED). https://www2.ed.gov/policy/gen/guid/fpco/ferpa/index.html

