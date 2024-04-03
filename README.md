# JavaScript-Assignment
The file data.csv  is a survey response file. 

Step 1: Preprocessing data: 
1. Remove duplicates.
2. Remove empty lines.
3. If there are more than one response for a student, get the latest response.
4. Convert the subject name, and club name that was submitted in the survey to the existent subject, or club name in subject_club.json. If the subject name or club name is not found in the subject_club.json, then the subject name or club name will be replaced with "Others".
  Ex: ["PE", "Sport", "Fitness", "Physical EducAtion", "Physical Education", "physical education", "Physical Education (Sports & Fitness)"] => Physical Education (Sports & Fitness)
5. Convert the CSV file to JSON file with schema as below:

|JSON Object |JSON Object|JSON Object|Required|
|------------| --------- |-----------|--------|
|questions   |order      |           |yes     |
|questions   |question   |           |yes     |
|responses   |student_id |           |yes     |
|responses   |age        |           |yes     |
|responses   |gender     |           |yes     |
|responses   |answers    |question_id|yes     |
|responses   |answers    |answer     |no      |


Step 2: Analyzing data:

6. Which subject does the youngest student like the most?
7. Which subject is the most popular among male students?
8. Which club is joined by the most female students as their extracurricular activities?
9. Which subject is the most popular among the students who joined the "Chess" club?
10. What is the percentage of the students who completed the survey?
11. What is the percentage of the students who like "Mathematics & Statistics" subject?
