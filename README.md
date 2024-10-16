# cassandra


# Music Streaming Data Analysis using Cassandra
Overview
This project involves creating a NoSQL database using Cassandra to analyze user activity and song data from the music streaming app SoundCloud. The goal is to address the inefficiencies of using a CSV file by migrating the data to a more query-friendly NoSQL format. The data will be modeled and queried using Apache Cassandra to answer specific questions regarding user behavior and song preferences.

Project Objectives
Data Modeling: Transition the data from a CSV file to a Cassandra NoSQL database.
Data Queries: Solve three specific queries about user activities on the platform using the NoSQL database.
Technologies Used
Python: For data processing and query execution.
Apache Cassandra: As the database solution for efficient data management.
Pandas: For CSV data manipulation.
Docker: For running Cassandra on Windows as if on a Linux OS.
CQL (Cassandra Query Language): For creating tables and querying data.
Installation
To run the project, you will need to install the following dependencies:

```bash
Copy code
pip install pandas cassandra-driver
```
Ensure that you have Apache Cassandra installed and running locally or remotely. You can download it from here.

Running the Project
Clone this repository to your local machine:

```bash
Copy code
git clone https://github.com/shadrach098/cassandra.git
```
Download and install Docker from here.https://docs.docker.com/desktop/install/windows-install/

Navigate to the project directory and start the Apache Cassandra service using Docker Compose:

```bash
Copy code
cd your_repository
docker-compose up -d  # Start the Cassandra service
```
To stop Cassandra, run:

```bash
Copy code
docker-compose down  # Terminate the Cassandra service
```
Open the Jupyter Notebook and run the cells in sequence to execute the data import, processing, and queries.

Follow the comments and explanations in the notebook to understand the problem-solving process and the results of each query.

Dataset
The dataset event_data.csv contains records of user activity from the SoundCloud app. This dataset will be used to populate the Cassandra database for querying.

Queries Addressed
Query 1: Find the artist_name, song_title, and length of the song heard in session number 338 and item in session number 4.
Query 2: Find the artist_name, song_title (sorted by item in session number), and the user's full name (fname and lname) for user_id = 10 and session_number = 182.
Query 3: Find every user (fname and lname) who listened to the song title 'All Hands Against His Own.'
Conclusion
By the end of this project, you'll have modeled the music streaming data in Cassandra, answered key queries regarding user activity, and optimized the system for easier data analysis.


