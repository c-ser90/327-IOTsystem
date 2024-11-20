CECS 327 Intro to Networking and Distributed System
Assignment 8: Build an End-to-End IoT System
IoT (100 points)
Due Date: Mentioned below
Build an End-to-End IoT System
Objective
In this assignment, you will build a complete end-to-end IoT system as shown in Figure
1. This project will integrate the TCP client/server you created in Assignment 6, your
database from Assignment 7, and IoT sensor data to process and analyze user queries.
You are also expected to incorporate metadata for each IoT device created in dataniz to
enhance the system's functionality.
Learning Objectives
By completing this assignment, you will:
1. Learn how to integrate IoT sensors and databases into a functional system.
2. Improve your TCP client-server communication skills with real-world IoT data.
3. Understand and utilize metadata for IoT devices to enhance system flexibility.
4. Perform data analysis and unit conversions in response to user queries.
5. Gain hands-on experience with cloud deployment and system integration.
CECS 327 Intro to Networking and Distributed System
Assignment 8: Build an End-to-End IoT System
IoT (100 points)
Due Date: Mentioned below
Assignment Requirements
Step 1: Modify the TCP Client
Update your TCP client from Assignment 6 to:
• Accept and process the following three queries only:
1. What is the average moisture inside my kitchen fridge in the past three hours?
2. What is the average water consumption per cycle in my smart dishwasher?
3. Which device consumed more electricity among my three IoT devices (two
refrigerators and a dishwasher)?
• Reject any other input with a user-friendly message, e.g., 'Sorry, this query cannot be
processed. Please try one of the following: [list the valid queries].'
• Send valid queries to your TCP server for processing.
• Display results from the server to the user.
Step 2: Modify the TCP Server
Update your TCP server from Assignment 6 to:
• Connect to the database created in Assignment 7 to retrieve relevant IoT data.
• Use metadata for each IoT device created in dataniz to manage and process queries
effectively. Metadata might include device ID, data source type, time zone, and unit of
measure.
• Perform calculations or unit conversions where needed:
- Convert moisture readings to RH% (Relative Humidity).
- Provide results in PST and imperial units (e.g., gallons, kWh).
• Use an efficient data structure (e.g., binary tree) for searching and managing the data.
Step 3: IoT Sensor Research
Research and document the IoT sensors you selected last week:
• Describe the types of data generated by each sensor (e.g., moisture, electricity
consumption, water usage).
• Explain the unit of measure, data precision, and time zones.
• Clearly indicate how metadata for each device from dataniz has been used in your
system. If you choose not to use metadata, you must explain your reasoning in your
report and presentation.
Deliverables
This is a group assignment. You will work with the same group chosen in Canvas. Your
group is responsible for the following:
1. Code Submission:
- Submit a GitHub repository containing your project code. Ensure:
• All code compiles without errors.
CECS 327 Intro to Networking and Distributed System
Assignment 8: Build an End-to-End IoT System
IoT (100 points)
Due Date: Mentioned below
• The repository includes detailed README instructions on how to run the client,
server, and database.
• Metadata for IoT devices from dataniz is integrated, or a justification is provided for
not using it.
• Invite the ISA to your GitHub repo. Commits will be reviewed to evaluate individual
contributions.
2. Presentation:
- Prepare a 5-10 minutes demo and presentation for the class. The demo should:
• Showcase your system’s functionality.
• Explain how metadata from dataniz was used to enhance the system.
• Provide reasoning if metadata was not utilized in certain parts.
• Highlight challenges encountered and how you resolved them.
• Include feedback on your experience using dataniz.com and suggest at least one
feature or improvement for the platform.
3. Report:
- Submit a concise report (maximum 2 pages) that includes:
• A summary of your system architecture and approach.
• Research findings on IoT sensors and data.
• A section detailing how dataniz metadata was used, or an explanation of why it was
not applicable.
• Details of any algorithms, calculations, or unit conversions impleme nted.
• Challenges faced and how they were addressed.
• A section on your feedback for dataniz.com.
Important Notes
1. All queries must be processed in PST and presented in imperial units.
2. Pay close attention to the sensor data you’re using. Ensure it is relevant, realistic, and
matches the query requirements.
3. Metadata integration is a critical component. If metadata is not used in a specific part
of the system, you must provide a clear explanation and justification.
4. Ensure that your virtual devices on Dataniz are turned on and configured to capture
data at various times during the day. This will help generate realistic datasets for query
processing and analysis.
Grading Criteria
Your submission will be graded as follows:
• Functionality (30%): Does the system correctly process queries, interact with the
CECS 327 Intro to Networking and Distributed System
Assignment 8: Build an End-to-End IoT System
IoT (100 points)
Due Date: Mentioned below
database, and return accurate results?
• Metadata Usage (10%): Is metadata from dataniz appropriately integrated? If not, is the
reasoning valid and explained clearly?
• Code Quality (20%): Is the code readable, modular, and well-documented? Are
commits meaningful?
• Presentation (20%): Does the team clearly explain the system, demonstrate
functionality, and provide insightful feedback on dataniz.com?
• Report (20%): Is the report well-written, structured, and aligned with the system demo?
Timeline
1. GitHub Repository Submission: (11/21/2024)
2. Presentation Date: (Sec 1 (12/03/2024), Sec 2 (12/04/2024))
3. Report Submission: (12/08/2024)
Hints & Tips
• Metadata can significantly improve query processing and data organization. Think
creatively about how to use it in your system.
• Collaborate effectively as a team and divide tasks evenly to ensure all group members
contribute.
• Document your approach and decisions as you work to make the presentation and
report easier to prepare.