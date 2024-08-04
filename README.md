# Darren Small T2A1-A, WORKBOOK PART A

### Question 1 Answer:
- The typical architecture of a API project, such as a flask application with Python, would be using the MVC design pattern. MVC stands for Model - View - Controller and divides an applications architecture into these 3 main components. Looking at each of these components and their specific roles:
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

### Question 2 Answer:
- A commonly used database in an API project, such as a flask application with Python, would be using a PostgreSQL database. The pros and cons of using this type of database are:
    - Pros:
        - it is open source and freely available, allowing the freedom of use to implement and modify according to the project needs. Because of this active and open source community it is continually updated and improved on for better solutions.
        - Postgres is highly extensible. What this means is the database can easily be extended, it is not fixed, so any new custom data types, functions, operators and languages can easily be added as required.
        -  
