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

        - Microsoft Commerce and Ecosystems division were having issues with most engineers still using a mixture of both the waterfall and scrum methodologies. They were constantly missing sprint conclusions and had a need to visualize their work, which scrum could not provide. So they decided to transition across to the kanban method. The kanban method and its visual nature made it easier for the entire team to see what needs to be done, wheather it was a newcomer to the team, someone back from vacation or a part timer, all team members could visually identify whats next on the kanban board. The results were a smoother process, happier customers and a team that worked well together. The article and reference can be viewed form this link:

        - [Deploying Kanban at Microsoft leads to engineering excellence](https://www.microsoft.com/insidetrack/blog/deploying-kanban-at-microsoft-leads-to-engineering-excellence/)

References:

Rehkopf, M. Atlassian. Kanban vs. scrum: which agile are you? [Online]
Available at: https://www.atlassian.com/agile/kanban/kanban-vs-scrum

GeeksforGeeks. 2024. Kanban vs. Scrum : Top Differences You Should Know [Online]
Available at: https://www.geeksforgeeks.org/difference-between-scrum-and-kanban/

## Question 4 Answers:

A standard source control process for an API project will be using Git and Github.












