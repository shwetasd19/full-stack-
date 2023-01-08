# full-stack-

##https://frontend-task-438b1.web.app/

Start by setting up a new ReactJS project. This can be done using the Create React App tool.

Next, create mock datasets based on the given data. These datasets should have the same time-series as the original data, but with different values.

Once you have the mock datasets, you can begin building the visualizations. For the first visualization (comparing data from three locations), you can use a chart library such as Chart.js or D3.js to create bar charts or line graphs. For the second visualization (filtering data by time range), you can use a date picker or range slider to allow the user to select a time range. For the third visualization (time-series graph with overlaid PM readings), you can use a line chart to plot the data. Finally, for the fourth visualization (showing the most windy days of the week), you can use a bar chart or pie chart to display the data.

To enable/disable dark mode, you can use the useState hook in React to manage the state of the dark mode toggle. When the toggle is clicked, you can update the state and apply a dark theme to the page using CSS.

To create separate views for the time-series and comparison graphs, you can use React Router to create different routes for each view.

To deploy the dashboard, you can use Heroku or Firebase Static Website hosting.

For the backend task, I would recommend the following steps:

Start by setting up a new ExpressJS project with TypeScript. You can do this using the Express Generator tool.

Next, create a suitable data model for the given data. This data model should include fields for the device id, timestamp, windspeed, wind direction, and PM particle values.

Use MongoDB as the database for the API, and connect to it using the Mongoose library.

Create the CRUD routes for the API. For the "pull data for specific devices" route, you can use a MongoDB query to filter the data by device id. For the "pull PM values separately" route, you can use the MongoDB aggregation pipeline to group the data by device and calculate the sum of the PM values for each device. For the "filter data by time range" route, you can use a MongoDB query with a date range filter to retrieve only the data within the specified time range. For the "upload bulk data" route, you can use the Multer library to handle the file upload and then parse the data from the Excel sheet using a library such as XLSX or XLS.

Implement the repository pattern for organizing the database operations. This will allow you to separate the database logic from the controller logic and make the code easier to maintain.

Use JWT tokens to authenticate the API calls.

As a bonus, you can consider containerizing the stack using Docker. This will allow you to easily deploy the API in a production environment.
 
