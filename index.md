
 Yiscah Mark

5 Fox Hill Rd, Spring Valley, NY 10977 | 914-705-9925 | Ymark@my365.bellevue.edu


[View My Resume](Resume.md)


Professional Summary:

A motivated and accomplished entry-level Data Scientist (4.0 GPA), whose mind and capable, hard-working nature enable
consistent high-performance in demanding technical environments. Paired with eager curiosity, a logical approach to
problem-solving, strong interpersonal skills, and articulate communication, these skills enable the delivery of impactful,
data-driven narratives.

**
Project One - [Resume Classification Project](notebooks/resumeclassnew (1).ipynb)
**

Project Objectives: The point of this project was to create a program that ingests various resumes and correctly categorizes them into the appropriate categories. I used a very large dataset from Kaggle with many prelabeled resumes, so the program could train itself to recognize and sort various resumes.


Programmatic Achievement When researching the dataset, it appears very simple and easy to work with. As soon as I started, I realized how unstructured and hard to work with it was, among other issues. Not one to give up, I pushed through without changing data in the middle. After achieving a very low accuracy of 53%, I improved the program by rewriting the ingestion logic to perform a safe split of the raw CSV lines and correctly organize them into a structured Pandas DataFrame. I converted the text into numerical data so the computer could process it using distance calculations. A computer can’t really understand language unless spoonfed in technical bite-sized pieces. When words are converted to vectors and numerical arrays, the computer can perform complex calculations to determine the distance and similarity between texts.


Observations: The famous saying about data is “garbage in, garbage out”. People expect data to be a magical answer to everything, a prediction of the future… While there is a lot of potential for data, if it isn’t of good quality, not much can be extracted from it. The beginning of my project was a great example of what not to do. My model scored 53% accuracy. This was likely due to label misalignment. I fixed this issue by implementing a safesplit function that specifically handles encoding errors. This step was essential to correctly align the resume text with its prospective category. There is a mathematical way to actually measure similarity between texts. The Euclidean distance measures the distance between vectors to determine similarity. A similarity of 0 indicates perfect similarity; thus, a value of 1.3 indicates that the resume classified as taught is very different from the one for Apparel. A critical piece of my NLP pipeline was to remove background noise and normalize the text. I removed all stopwords because they don’t give a unique meaning to the text. I also removed special characters because they made the text very messy, and I lowercased all the words to unify them. I also ran the text through the lemmatizer, which reduces all words to their root. By unifying all the text, the model can more easily detect patterns and similarities. This program successfully sorts resumes into categories. I learned how important data structure is and how to clean and remove noise from text so that similarities and nuances are clearer. This achieves the object of turning unstructured data into workable material to provide a scalable solution for processing large volumes of professional documents.

Project One - [COVID E-commerce Project](project2.md)
Summary: The COVID E-commerce Project was a time series model created to visualize and explore changing trends of e-commerce in the years post COVID-19. The model shows a very clear skyrocketing of e-commerce amounts right in the beginning years of COVID. The chart is grouped and color-coded by time group for clarity. Before, During and After COVID. Another model is divided by jump in amounts of e-commere per specific category.
