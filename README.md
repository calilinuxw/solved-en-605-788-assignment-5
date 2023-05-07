Download Link: https://assignmentchef.com/product/solved-en-605-788-assignment-5
<br>
The goal of this assignment is to learn to write a more complicated MapReduce program for processing big data sets in parallel using MapReduce framework.




<ul>

 <li>Create a MapReduce program called MovieRatings that will print all the average ratings for a movie based on user feedback</li>

 <li>The program should work on MovieLens data set, which can be downloaded from http://www.grouplens.org/node/73. Download the 100k data (ml-100k.zip) set into your Downloads folder. Extract the  ml-100k.zip file into ~/Downloads folder itself.  For this particular assignment, the program will use the u.data and u.item files under the extracted folder.  Technically speaking, you really do not have to do this step if you had already done assignment 3. Because this was data preparatory step for assignment 3.</li>

 <li>On running the MovieRatings MapReduce program, it should process the u.data file, which contains a list of movie ratings by users and also process u.item file, which has movie related information. In the u.data file, each user has rated at least 20 movies. Users and items are numbered consecutively from 1.  The u.data file is randomly ordered and the fields are tab separated with list of fields being user id, item id, rating and timestamp. The u.item field contains sveral pieces of information about each movie.  The u.item file is pipe(|) separated.  Unfortunately, the text of the README file is incorrect in terms of field separator for u.item, but it has the correct information about the fields and their order.  Please look at the actual file and also the README file.</li>

 <li>The program should take 2 arguments. The first argument should be the directory where the movielens user data set (u.data) and movie information (u.item) files are placed (called /movie-and-ratings in hdfs), and the second argument is the name of directory where the results will be placed in HDFS (called /movie-rating-result).</li>

 <li>The result of the program should be a list of all movies rated with the following information per line — movie id, movie title, release date, IMDB URL, average rating, total number of unique users rated, total number of ratings for the movie</li>

 <li>Use 2 reducers by setting the number of reducers to 2.</li>

 <li>Write a combiner for efficiency, if possible</li>

 <li>Define a custom counter that has a running count of total records processed in map, total number of unique movies in reducer.</li>

 <li>Before you begin, please split the input file into 5 files called u1.data, u2.data, u3.data, u4.data and u5.data, each having 20000 records. Use the Unix split command.</li>

</ul>

Reference: https://kb.iu.edu/d/afar

<ul>

 <li>All the input files – 5 user ratings file and the movie information file should be gzip compressed before processing.</li>

 <li>Reducer output files should be gzipped.</li>

</ul>




<strong>What to turn in? </strong>

<ul>

 <li>Jar file that can be run at command line</li>

 <li>A zip of NetBeans or Eclipse project</li>

 <li>A sample run with output as a Word document. I have given you a template for assignment 4 solution. Follow the guidelines, fill the document and submit.</li>

</ul>


