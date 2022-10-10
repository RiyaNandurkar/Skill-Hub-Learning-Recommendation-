# Skill-Hub-Learning-Recommendation-System:
Building a Simple Course Recommendation system for online courses

## About the Project
The Course Recommendation System Skill Hub recommends resources according to the needs of students, course streams that can be considered by students to excel in their field of interest, skill, recommendations on the basis of skills, ratings, students enrolled in the course.
  
 
## Dataset Used
For the purpose of building Skill-Hub, data from Coursera was scraped using the requests and beautifulsoup4 libraries. The ```scraper.py``` file contains code for scraping data from [https://www.coursera.org/courses](https://www.coursera.org/courses) and generates [coursera-courses-overview.csv](https://github.com/ry05/couReco/blob/master/data/coursera-courses-overview.csv). The ```course_scraper.py``` file contains code to scrape details of each individual course and the output is [coursera-individual-courses.csv](https://github.com/ry05/couReco/blob/master/data/coursera-individual-courses.csv).  

Both these above datasets have been combined to give [coursera-courses.csv](https://github.com/ry05/couReco/blob/master/data/coursera-courses.csv). This file consists of 1000 instances and 14 features and has a size of 1.41 MB.

### Features in the Dataset
The following features have been extracted for the dataset created above:   
**course_url:** The URL to the course homepage  
**course_name:** The name of the course  
**learning_product:** The type of product that the instance is. It can be a course, professional certificate or a specialization. *(While all instances of the dataset are referred to as courses, this is not be confused with the learning_product of a particular instance) *  
**course_provided_by:** The organization/partner that is providing the course  
**course_rating:** Overall rating of the course  
**course_rated_by:** The number of students who have rated the course  
**enrolled_student_count:** The number of learners who have enrolled into this course  
**course_difficulty:** The difficulty level of the course. It can take values of beginner, intermeditae, advanced and mixed  
**skills: ** The main skills that the course works at developing in a learner  
**description: ** About the course  
**percentage_of_new_career_starts:** Percentage of learners who have had a new career start after completing this course  
**percentage_of_pay_increase_or_promotion:** Percentage of learners who have had a pay increment or received a promotion after completing this course  
**estimated_time_to_complete:** The estimated tome to complete the course  
**instructors: ** The instructors taking the course  


## Usage
The instructions to run Skill-Hub on your local system are as follows:

1. Create a virtual environment on your local system to install this project's dependencied and run it
2. Download or clone this repository into your virtual environment
3. Run the following command to install necessary libraries for Skill-Hub to run
  
4. Run the streamlit app with
  ```
  streamlit run streamlit_app.py
  ```
5. The app should open at http://localhost:8501(can be different)

## Screenshots
Added with other files.

## What can Skill-Hub do?
In a nutshell Skill-Hub can perform the following tasks:
* Select courses for you based on the skills you want to learn
* Recommend courses that are most similar to the course you select

## References
If you liked the concept and implementation of Skill-Hub, do check out the following resources that provided me with some much needed help while working on this:
* [The Streamlit Official Guide](https://www.streamlit.io/)
* [The Real Python Guide to using Beautiful Soup](https://realpython.com/beautiful-soup-web-scraper-python/)
* Adomavicius G, Tuzhilin A. Toward the next generation of recommender systems: a survey of the state-of-the-art and possible extensions[J]. IEEE Transactions on Knowledge and Data Engineering, 17(6): 734-749, 2005
* Park D H, Kim H K, Choi I Y, et al. A literature review andclassification of recommender systems research[J]. ExpertSystems with Applications, 39(11): 10059-10072, 2012 
* Lecuny, Bengio Y, Hinton G. Deeplearning. Nature, 521(7553): 436-444, 2015 

