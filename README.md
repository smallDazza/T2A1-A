# Darren Small T2A1-A, WORKBOOK PART A

## Question 1 Answer:
The typical architecture of a API project, such as a flask application with Python, would be using the MVC design pattern. MVC stands for Model - View - Controller and divides an applications architecture into these 3 main components. Looking at each of these components and their specific roles:
    - Model: The model component contains all the logic relating to data, so the user can interact with the database. It is the only component able to connect to the database and the model only communicates with the controller and responds with the requested data from the database to the controller as required. It can provide all the data related actions from the user being transferred between the view and controller.
    - View: The view component provides all the UI interactions of the application for the users inputs and display outputs. It only communicates with the controller to provide a view of the data from the model.
    - Controller:   The controller component contains all the core logic and is the main processor of the application. It connects the view and model components and is the interface between them for taking requests from the view to manipulate data through the model. It then has the logic to provide the view with the correct rendered output to display to the user.

An example of a application with this type of architecture could be a weather app:

    1 - The user opens up a web browser and goes to the weather applications main page. This is the View or the UI component. User interacts with the View and enters the locations and days they would like to know the weather outlook for.

    2 - The View sends this request to the Controller to get the weather information.

    3 - Then the Controller requests the Model to find this weather information from the database.

    4 - The Model finds all the information from the database and returns this to the Controller.

    5 - Then the Controller decides how to display this information to the user and advises the View on how to render this data for display.

References:

Pratap M., 2024. How does the Python MVC Framework Work [Online]
Available at:  https://supersourcing.com/blog/how-does-the-python-mvc-framework-work-what-are-the-benefits/

GeeksforGeeks., 2024. MVC Design Pattern [Online]
Available at:   https://www.geeksforgeeks.org/mvc-design-pattern/

Kumar N., 2021. How the Model View Controller Architecture Works [Online]
Available at:   https://www.freecodecamp.org/news/model-view-architecture/

## Question 2 Answer:
A commonly used database in an API project, such as a flask application with Python, would be using a PostgreSQL database. The pros and cons of using this type of database are:

    - Pros:
        - It is a RDBMS system compliant with SQL standard making it easy to use for developers and users familiar with SQL.
        - Postgres became ACID compliant in 2001, meaning it has the 4 properties of atomicity, consistency, isolation & durability, making it well known for its reliability. It can handle a large amount of data while being highly stable and not crashing or losing data. This maintains data integrity and does offer write ahead logging, to prevent data loss, as well as crash recovery procedures.
        - Postgres is highly extensible & flexable. What this means is the database can easily be extended, it is not fixed, and supports a wide range of inbuilt data types as well as any new custom data types, functions, operators and languages can easily be added as required.
        - It is highly scalable. Postgres can be run on a single server or multiple servers to manage large amounts of data. It can also handle a large number of concurrent users making it the ideal choice for large applications requiring both these features.
        - Has MVCC - Multi Version Concurrency Control which enables the use of multiple transactions accessing the same data simultaneously with out any issues.
        - Postgres security is very high with role based access controls, secure connections and data encryption available.
        - Postgres can support data warehousing and business intelligence tasks with advanced analytics & data visualization.
        - It is open source and freely available, allowing the freedom of use to implement and modify according to the project needs. Because of this active and open source community it is continually updated and improved on for better solutions.
    
    - Cons:
        - Postgres performance can be slower than other database systems when performing certain types of data structures or queries.
        - For new users and developers it can be quite complicated and hard to learn. Because the database is highly configurable, this type of complexity is a potentail drawback.
        - The Postgres documentation can be hard to navigate, as being open source there are a large volume of resources available and many tools support MySQL and not Postgres.
        - Migrating data from other databases is challenging and difficult, especially for large amounts of data.

References:

BrainerHub Solutions. 2023. PostgreSQL: A Practical Guide—Features and Advantages. [Online]
Avaliable at: https://www.linkedin.com/pulse/postgresql-practical-guidefeatures-advantages-brainerhub-solutions

Quest. What is PostgreSQL and how does it compare to other database management systems? [Online]
Available at: https://www.quest.com/learn/what-is-postgresql.aspx

Nguyen, H. 2024 What is PostgreSQL and Everything You Need to Know. [Online]
Available at: https://techvify-software.com/what-is-postgresql/

Vojak, J. 2022. Exploring the pros and cons of SQL databases — MySQL, Postgres, Oracle, Microsoft SQL, and Amazon Aurora. [Online]
Available at: https://josipvojak.com/exploring-the-pros-and-cons-of-sql-databases-mysql-postgres-oracle-microsoft-sql-and-amazon-3c8de880b8d4

## Question 3 Answers:
The implementation of an Agile project management methodology for an API project would be to use either the SCRUM approach or the KANBAN approach. But the approach to choose ultimately dpends on the type of API project being undertaken, the development team in place and the project outcomes for the client. Below is a description of each Agile approach and example(s) of a real world example where businesses have applied this to their own software/api projects:

- SCRUM: 

    Scrum methodology for projects is where the team promises to achieve and deliver a piece of project work by the end of a certain amount of time, called a sprint. Sprints usually last for a length of time between 1 to 4 weeks. The team usually consists of a Product Owner, Scrum Master and the development team members. The task for the sprint will be broken down into smaller tasks called 'stories' where each development team member will be assigned their 'story' to work on for that particular sprint.

    The scrum master works together with all dev team members to help them stay focused, resolve any issues and keep the sprint task to its designatd timeframes. This is usually done by also running regular daily team meetings.

    The product owner prioitzes the tasks for the dev team and the backlog of the project. They also liaise with the client in regards to the overall progress of the project and any changes or concerns they have for their overall outcomes of the project.

    At the end of each sprint task goal, the whole team will come together to review, plan ahead for future sprints and retrospectively analyse what went well and not so well for this task.

    Scrum real world example:

    - Salesforce:

        - Salesforce embraced a scrum methodology for its cloud based products back in late 2006. Before this, and the reason for their change, was because they had seen their seasonal releases slip from 4 per year, when first started, go down to just one per year. So they knew they had to change their development methodology. Since adopting a scrum methodology in late 2006, by 2010 each major release had been successfully delivered on the exact day as scheduled and their customer satisfaction indicator was at 94%. Another scrum advantage they saw was an increase in productivity, measuring by features produced per developer, they saw an increase of 38%. The case study white paper done on this in 2010 can be reviewed from this link: 

        - [The inside story of salesforce.coms transformation from waterfall to agile](https://web.archive.org/web/20110429103410/http://www.ca.com/Files/WhitePapers/wp-agile-development_239775.pdf)

- KANBAN:

    Kanban methodology for projects is more a visual signaling mechanism where the workflow is represented on a kanban board by tasks that will flow from one stage of the workflow to the next stage. For example, the most commmon workflow or columns of each stage are 'To Do', 'In Progress', 'In Review' and 'Done' but these are most often customised by the development team for each specific project. 
    
    When each task has been reviewed / accomplished by a development team menmber at a stage on the kanban board, they will move the task to the next stage until the outcome of 'Done' is achieved. Depending on the size of the project and the development team, each stage could be assigned and achieved by the same team emeber or different team members.

    With kanban, releases or updates are done when they are ready, not based on predetermined dates or a regular schedules like scrum. The whole development team works together and owns the kanban board to achieve the projects outcomes. Because of this, the most common practice to deal with issues or blockages, is to implement  Work In Progress (WIP) limits, where caps are placed on the number of tasks that can be placed in any particular column. When the cap or limit is reached the whole team can work together to resolve the tasks that stalled the workflow process.

    Kanban real world example:

    - Microsoft:

        - Microsoft Commerce and Ecosystems division were having issues with most engineers still using a mixture of both the waterfall and scrum methodologies. They were constantly missing sprint conclusions and had a need to visualize their work, which scrum could not provide. So they decided to transition across to the kanban method. The kanban method and its visual nature made it easier for the entire team to see what needed to be done, wheather it was a newcomer to the team, someone back from vacation or a part timer, all team members could visually identify whats next on the kanban board. The results were a smoother process, happier customers and a team that worked well together. The article and reference can be viewed form this link:

        - [Deploying Kanban at Microsoft leads to engineering excellence](https://www.microsoft.com/insidetrack/blog/deploying-kanban-at-microsoft-leads-to-engineering-excellence/)

References:

Rehkopf, M. Atlassian. Kanban vs. scrum: which agile are you? [Online]
Available at: https://www.atlassian.com/agile/kanban/kanban-vs-scrum

GeeksforGeeks. 2024. Kanban vs. Scrum : Top Differences You Should Know [Online]
Available at: https://www.geeksforgeeks.org/difference-between-scrum-and-kanban/

## Question 4 Answers:
A standard source control process for an API project will be first the project development team needing to use / deciding to use a version control systems software. This VCS software is used by the development team to manage changes in the projects source code over the length of time the project takes to complete.
The development team process for the VCS of the project will be applying a number of standard practices, these are:

    - Repository setup: organising the structure of the code into clear and consistent repositories.
    - Branching strategies: to manage code changes a good branch strategy is required. This could be having a 'main' branch for production ready code, a 'dev' branch for ongoing developement and testing, then creating new branches as required for future version releases or bug fixes where these can be merged back into the main branch when finished.
    - Commit messages & frequency: when team members are commiting changes they need to write concise and informative messages. This way other members of the team will know and understand what they have done. Members should also be instructed to make regular frequent small commits rather than infrequent larger commits. This makes tracking changes and identification of bugs easier for all team members.
    - Using pull requests: team members should use pull requests for all code changes. These pull requests can be used for reviewing code, testing and code quality reviews before merging them back into the 'main' branch.
    -  CI/CD processes: a Continuous Integration/Continuous Deployment process should be implemented. This involves a pipeline to trigger the automation of the building, testing and deployment of code changes to the dev environment.
    - Resolving conflicts: all team members should work together to resolve any merging conflicts quickly when they happen. These conflicts happen when different members have modified the same part of a file.
    - .gitignore: To specifically have any file or directories ignored by the VCS software, member should use a .gitignore file.
    - Security: access control measures should be used by the dev team to protect the main production branch. This security should help prevent things like deletions, direct pushing to production and unauthorised access.
    - Cleanup process: a branch cleanup process should be regularly done to remove old & unused branches. This will maintain a managable and clean repository.
    - Documentation: The repository should include a documentation file or README file to guide any new or current dev team members of the processes of building, running, testing and cloning any part of the software project.

Examples of VCS software tools available in the market are:

    1. Git: Git is a open source VCS software that tracks the project changes, staging areas and commits these to the repository. It is the most widely used VCS system in the world and has become a standard in the software development industry.
    2. GitHub: GitHub is a cloud based hosting service tool that hosts the Git repositories. GitHub provides a wide variety of different VCS features for collaboration and access control. It is owned by Microsoft and tends to be used for more open source community public code access.
    3. BitBucket: is a very similar VCS Git repository management tool with all the same features as GitHub but tends to more widely used for the private business sector. It is owned by Atlassian.
    4. AWS CodeCommit: this is AWS (Amazons) version of a VCS Git repository management tool.

Examples of projects using VCS via GitHub:

    1. This link provides a basic GitHub repository template & example and can be used to create a well documented README file:
[GitHub Call-for-Code / Project-Sample](https://github.com/Call-for-Code/Project-Sample)

    2. This link is the Ruby on Rails platform project. This has 5000+ contributors & 92380 commits to date:
[GitHub rails / rails](https://github.com/rails/rails)

    3. This link is the facebook / react platform project. This has 1646 contributors & 19245 commits to date:
[GitHub facebook / react](https://github.com/facebook/react)

References:

Atlassian, 2024. What is version control? [Online]
Available at: https://www.atlassian.com/git/tutorials/what-is-version-control

Masal, B. 2023. Best Practices for Effective Source Control (version control) in Software Development. [Online]
Available at: https://www.linkedin.com/pulse/best-practices-effective-source-control-version-software-balaji-masal-agxpf

Indeed. 2024. Source control: definition, importance and examples. [Online]
Available at: https://uk.indeed.com/career-advice/career-development/source-control

mattfarina. 2024. Large Projects on GitHub [Online]
Available at: https://gist.github.com/mattfarina/7627cb5ebb8fc01bfd62f4a6942fce04

## Question 5 Answers:
For a standard testing process for a API project, the development team will first have to either write their own framework or choose from a number of API software testing tools. Some of the most common API testing tools available are:

- Postman API Platform.
- Amazon API Gateway.
- Google Apigee.
- Insomnia by Kong.
- Swagger from SmartBear.
- Microsoft Azure API Management.

The development team will then decide on the types of tests required for their application by verifying the functionality & performance of the API. The most common types of API tests are:

- UI testing: not specific to an API but this testing is important for the applications integration between the user interface (front end experience) and the API (back end functionality). This type of testing is usually a manual process.
- Functional testing: this testing ensures the API functions in the exact way it is designed to for the application. It is done by verifying that the correct responses and data formats are returned by the API from specific requests. These tests should include:
    - status code verification: the correct status codes are returned eg; 200, 404 etc.
    - response data validation: the responses include all the correct data fields & values.
    - date accuracy: data returned is as expected & accurate.
    - error handling: all errors are handled correctly and display meaningful messages.
    - operates using CRUD: all create, read, update and delete functions works as expected.
- Performance testing: this testing ensures the API can perform and handle large volumnes of data and traffic. It is done by replicating multiple users with multiple requests so the API will be under load and then measuring its performance. These tests should include:
    - load test: replicating high user traffic to measure speed & responsiveness times.
    - response time: measuring the time to respond between different loads eg; normal & peak loads.
    - scalability: when increasing the load and users, testing how it scales.
- Security testing: this testing ensures the API is secure. It must be able to prevent any unauthorized access and protect the applications sensitive data. This is done by executing tests to identify any vulnerabilities in the API system. These tests should include:
    - authentication: verifying the proper authentication and manages invalid credentials correctly.
    - authorization: verifying all users can only have access to the data they can modify or view.
    - input validation: tests like SQL & command injection to validate all inputs.
    - data encryption: testing the data during transmission is encrypted.  
- API documentation testing: this type of testing is used to determine that the API documentation accurately reflects its capabilities and all its features work as expected for the projects application. Similar to functional testing but could be incorporated with tests that include:
    - ease of use: verifying the API integrates well and is easy to use.
    - naming conventions: checking the naming conventions of all endpoints and parameters are consistent.
    - document accuracy: verify the documentation is up to date and accurate for the API.

Examples of real world API testing:
- a airline booking site application like skyscanner, needs to display to the user all the correct airline flight details, dates and rates in a timely manner. To do this it must effectively communicate with all the different airlines API's. The skyscanner development team must regularly do the above API tests to ensure their website application is successfully communicating with all the different airlines API services and returning the correct results in a acceptable timeframe. Should the user also then decide to purchase a certain airline product they must ensure the users personal details are effectively secure and correctly sent to the airlines boooking system. 

- another example is the company i work for called myPak Solutions. MyPak provides a packing application for pharmacies around Australia to print their patients prescribed medication details on a blisterpack packaging supplied by the pharmacy, so they can effectively take their medications in a safe manner, reducing the chance of dependency or overdosing. To do this the myPak application must have access to the pharmacies medication dispensing programs data, which is done via their API's.
Their are currently 6 dispensing medication software companies in Australia and 4 of them provide access to their data via their own API's. MyPak's development team regularly use the same above API tests to ensure that patients medication data its packing application is accessing is correct, secure and achieved in a timely manner. 

References:

Yasar K, Gillis A. 2024. What is API testing? Everything you need to know. [Online]
Available at: https://www.techtarget.com/searchapparchitecture/definition/API-testing

Codeheart I. 2023. API Testing: A Guide for Developers. [Online]
Available at: https://caisy.io/blog/api-testing-for-developers

Testsigma. 2024. API Testing : What It is, How to Test & Best Practices. [Online]
Available at: https://testsigma.com/guides/api-testing/

## Question 6 Answers:
The 3 principles of information system security are explained below and known as the CIA triad:

1. Confidentiality: this principle is to ensure that unauthorised users cannot accces sensitive / personal information & data. Measures must be put in place to ensure only authorised users can access this type of information and any other user is restricted , so that this type of data will remain confidential. One of these measures would be to check the authorisation levels of all users that have access to the applications data.

2. Integrity: this principle is to ensure the data is accurate, consistent and trustworthy. Measures are required so that no modifying of the data is done in transmission either accidently or intentionaly by malicious attacks, or by any unauthorised users.

3. Availability: this principle is to ensure that data is available to the authorised users of the application within a given timeframe. The timeframe availability is determined by the use case of the application but all technical infrastructure & hardware must be maintained, online and backed up to meet these expectations.

References:

GeekforGeeks. 2022. Principle of Information System Security. [Online]
Available at: https://www.geeksforgeeks.org/principle-of-information-system-security/

Milkovski I. 2022. What are the 3 Principles of Information Security? [Online]
Available at: https://www.linkedin.com/pulse/what-3-principles-information-security-igor-milkovski-m-a

Hashemi-Pour C. CIA triad (confidentiality, integrity and availability). [Online]
Available at: https://www.techtarget.com/whatis/definition/Confidentiality-integrity-and-availability-CIA

## Question 7 Answers:
The implementation of the 3 CIA triad principles of information system security in an API project is essential and in most cases must be done to meet local and international privacy laws. To achieve all 3 principles in any API project the following measures should be implemented:

- data encryption mechanisms: during data transmission this can be achieved by using secure protocols such as HTTPS. HTTPS will encrypt HTTP requests & responses with a technology called TLS. If an attacker were to access these HTTPS requests and responses they would only see random characters instead of the text being transmitted.
- password encryption techniques such as hashing: hashing is widely used in cryptography and is the process of converting any data into a fixed length hash that can never be reversed. This is why it is widely used for encrypting passwords. There are many different ways in coding to hash a password but one example, in the image below, is in Python to hash a password we can use the module called 'bcrypt':
![hash code example using the bcrypt module](./images/bcrypt%20code.png)

The red arrow indicates the encrypted or hashed password generated. The 'salt' variable in this code is a random input of additional one way data added to the hash for an extra layer of security.
- the use of checksum methods: to check the accuracy of data transmission over a system or network and that no changes, damage or errors have occured between the sender & receiver, a process called checksum can be used. The checksum method in coding is a algorithm that derives a value from the data, then compares this value at both the sender and recievers end. If there is any changes in the value it inidicates the unreliability of the data transmitted. This process verifies the integrity and authenticity of the API data. 
- keeping authorised user permissions & access control lists up to date: 
- using two-factor authentication for access to an application or API:
- a VCS (version control system) for application releases:
- backing up of data: 
- redundancy and failover measures:



















