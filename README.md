### Explore the Academicworld!

#### Haonan Shi's Final Project in CS411 2022

#### Purpose of this project:

This interactive dashboard is designed for those who are dedicated to the academic world and looking for academy searching engine for the mentor finding, paper searching and big picture getting from a board perspective to specific ones.  The dashboard will help students get a general of the academic world in an interesting and responsive way.

#### Demo:

The video demo of showing the basic infomation is: https://youtu.be/2Cyc-yF1TZs

#### Installation:

All that is required is to download all the codes(including the cache or else the first running may not working appropriately) and run the app.py like: "python app.py". If you are using Spyder like I did all the time, all you need to do is open the app.py file and run it. The Neo4j, however, needs to be turned on otherwises some functionalities will fail to work. All the data about the academic world should be stored in MySQL, MongoDB and Neo4j, as what we did in the previous machine problems.

#### Usage:

After running the code and go to http://127.0.0.1:8050/, a dashboard about the academic world will be visiable. All the six widgets are controllable by the user in some ways. For the graphs, users can zoom in to see the specific part. They can also choose the year in which the corresponding data will be given and shown. For the tables, users can choose which publication keyword or university they are interested in and the relevant datatable will show up. Users can do the qeury multiple times, if the program is run correctly. 

#### Design:

The dashboard is made with both frontend parts and backend parts.  

For the frontend parts(app.py),  We mainly use Dash and Plotly, which are two powerful packages used in Python. These two packages help to build a dashboard and offer some interactive ways for users to use and commnicate with the application, without know how the algorhithm works behind. As for the backend parts, we use three types of databases, MySQL(mysql_haonan.py), MongoDB(mongoldb_haonan.py) and Neo4j(neo4j_haonan.py), to build up our academicworld database for the users to query.  

#### Implementation:

**Frontend:** For the graphs, to make it interactive, responsive and updatable, Plotly package is very helpful can the Dash package can help create the graph on the dashboard. For the datatables, callback can offer great flexibility for the users to query. The power functionalities can also help read the photo Url of the faculty and show them on the dashboard. There are totally 6 widgets(**R6**), first two of which are updating widgets(**R7**), where you can zoom the data to see a specific part(users can also cancel this update by double clicking the graph). The last four are querying widgets(**R8**), where users can query as they want. All the widgets are arranged in a rectangular space in a simple way(**R9**).

**Backend:** I use all the *three databases* mentioned above to build the back end parts of the application. In order to make Python get access to all the three databases, several packages are gracefully helpful: mysql_connector(**R3**), neo4j(**R4**), pymongo(**R5**) and so on. The application is implemented in a useful and cool way(**R1** and **R2**).

#### Database Techniques:

I achieved four database techniques(**R10**,**R11** and **R12**): Indexing, view, stored procedure and parallel query execution. For some of the techniques, for example, creating an index, a view or a stored procedure, users only need to call it once. Otherwise an error will occur. The indexing technique is very useful for querying large datasets.The view is helpful when temperarily store the data to look at. A stored procedure is helpful just like the function in Python. Parallel query execution is helpful reduce the computation time.

#### Contributions:

Team name: Team Viewer

Team leader: Haonan Shi

Team member: Haonan Shi

Instruction: Kerui Zhu, Kevin Chang.

At the end of this great semester, I would like to express my appreciation to the professor and all the TAs(especailly Kerui, who helped me a lot). As a student who only knows how to deal with data and have zero knowledge about frontend application and language, I did feel the challenge when I received this project at the first time. It was very difficult for me to start. Approximately I spent about 50 hours on this project, and there are still many parts that can be improved, with no doubt. However, the great help of the professor and all the TAs helped me get through it anyways, and I do feel proud of myself. Honestly speaking, this is my first time to do a project like this, which conbines both frontend app and backend app.

One more time, thank you all for the great help, and thank you for reading this!