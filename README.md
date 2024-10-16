# cassandra

Music Streaming Data Analysis using Cassandra
Overview
This project involves creating a NoSQL database using Cassandra to assist with analyzing user activity and song data from a music streaming app, SoundCloud. The aim is to address the inefficiencies of using a CSV file by migrating the data to a more query-friendly NoSQL format.

The data will be modeled and queried using Apache Cassandra to answer specific questions regarding user behavior and song preferences.

Project Objectives
Data Modeling: Transition the data from a CSV file to a Cassandra NoSQL database.
Data Queries: Solve three specific queries about user activities on the platform using the NoSQL database.
Technologies Used
Python: For data processing and query execution.
Apache Cassandra: As the database solution for efficient data management.
Pandas: For CSV data manipulation.
CQL (Cassandra Query Language): For creating tables and querying data.
Installation
To run the project, you will need to install the following dependencies:

bash
Copy code
pip install pandas cassandra-driver
Ensure that you have Apache Cassandra installed and running locally or remotely. You can download it from here.

Running the Project
Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/your_username/your_repository.git
Navigate to the project directory:

bash
Copy code
cd your_repository
Open the Jupyter Notebook and run the cells in sequence to execute the data import, processing, and queries.

Follow the comments and explanations in the notebook to understand the problem-solving process and the results of each query.

Dataset
The dataset event_data.csv contains records of user activity from the SoundCloud app. This dataset will be used to populate the Cassandra database for querying.

Queries Addressed
create Three Different Database base on the following Queries:
Query 1:Find the artist_name, song_title and length of song the SoundCloud app history that was heard during  session_number = 338, and item_in_session_number  = 4
Query 2: Find the artist_name, song_title (sorted by item_in_session_number) and name(fname and lname) of the user for user_id = 10, session_number = 182    
Query 3: Find every name(fname and lname) of the user from the SoundCloud app history that listened to the song_title 'All Hands Against His Own'
Conclusion
By the end of this project, you'll have modeled the music streaming data in Cassandra, answered key queries regarding user activity, and optimized the system for easier data analysis.
