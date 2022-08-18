# MapperPublic

*Source code avaliable upon request.*  This was a project for a software design course that other students will be taking in the future (with a similar objective), hence the source is not public.

## Contributors
Mapper was a group project, split into groups of 3.  Alongside me were 2 super talented programmers mentioned below.

### Daniel Liu
GitHub: https://github.com/danielliucs  
LinkedIn: https://www.linkedin.com/in/danielliliu/  
Email: daniell.liu@mail.utoronto.ca  

### Hannah Ghassabeh  
GitHub: https://github.com/HannahGhassabyte  
LinkedIn: https://www.linkedin.com/in/hannah-ghassabeh-92200b204/  
Email: hannah.ghassabeh@mail.utoronto.ca  

### Dante Crescenzi
GitHub: you are on my github :)   
LinkedIn: https://www.linkedin.com/in/dante-crescenzi/  
Email: dante.crescenzi@mail.utoronto.ca  

## Demo Video
Below is a short demo of some of the features of mapper.  **More demos can be shown upon request :)**  Credit to my partner Daniel Liu for the amazing video.

https://user-images.githubusercontent.com/77305802/185508823-6eb70545-d24e-44e5-896a-7bb5951c3455.mp4

## Project Timeline
The mapper was divided up into 4 milestones, each with their own set of challenges and programming concepts to learn/practice.  They are listed below with a short summary

### Milestone 1 (M1)
* Milestone 1 consisted of parsing a large amount of OpenStreetMap (OSM) (https://www.openstreetmap.org/about) data and organizing it into appropriate data structures.  Many functions were then created for common GIS tasks, such as returning a list of possible matches of streets from a partial street name (ex, partial search 'ba' returning all streets starting with 'ba'), determining the length of any street, determining if any 2 intersections are connected (with one way streets to account for), and more.  All of the functions created had rigorous time complexity requirements, so proper data structure / algorithm choice was very important.

### Milestone 2 (M2)
* Milestone 2 consisted of adding a GUI to meaningfully display all of the geographical data that was processed in M1.  A graphics library 'EZGL' developed by the ECE297 teaching team was used, which was a wrapper for GTK3 and Cairo.  More can be seen here: https://github.com/mariobadr/ezgl.  Using the functions developed in M1 and EZGL, the team developed a GUI to visualize and interact with any map, from Toronto to New York to Beijing.  Features such as intersection highlighting, points of intrest, street names and more were required.  Our team completed all required features and added extra features such as subway visualization, autofocus to highlighted intersections, and autocomplete for intersection searching.  Optimization was important to make the map responsive.

### Milestone 3 (M3)
* Milestone 3 consisted of giving our map the capability of generating directions between any 2 points, teaching us programming concepts such as graphs, bfs & dfs, dijkstra's algorithm, A* and more in a practical way.  The directions also needed to be visualized.  Our team passed all performance tests, only capable through implementing an optimized A* algorithm.  Direction visualization can be seen in the demo above.

### Milestone 4 (M4)
* Milestone 4 consisted of implementing a solution for a modified travelling salesman problem, called the travelling courier problem.  It is practically planning out a route of a courier that needs to go around a city, picking up packages in one place and dropping them off elsewhere.  This milestone gave us a practical look at NP problem solving, greedy algorithms, multithreading, hill climbing, simulated annealling, and more.  M4 was fascinating, my personal favourite.

## What I'd Do Differently
With mapper being a induvidually team-managed term long project while juggling 4 other engineering courses, the development of this project forced us to make on the spot software architecture choices fast (which ended up being good experience :) ).  While I am proud and happy with our team's architecture choices that proved to be easy to build on and modular later in the project, there are a few things I would change:
* Less dependance on global variables - while we implemented globals in the safest way we could, minimizing globals is good form.  
* More use of OOP and Inheritance - some parts of the project, such as handling the displaying of many different types of object (road vs building vs point of interest, etc), could have leveraged the OOP of C++ and be made very clean, ex.  all objects inheriting from a class 'MapEntity'.
* Use of a planning tool such as JIRA - while our team did adopt the agile methedology, we did not use a tool such as JIRA to keep track of it all.  I have used JIRA in internships, and it would have helped here.

## Final Remarks
This project was a blast, and helped me learn so much.  From features of C++ itself to test driven development to the agile methodology to endless programming concepts such as algos, data structures, and more.  The teaching team and course itself was amazing.  As said above, source is avaliable upon request.  Cheers! :) 
