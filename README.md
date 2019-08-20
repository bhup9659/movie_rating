# This utility will let you know the rating of movies from OMDB API

PREREQUSITES:
First, create Docker environment is setup at the user end.

Second, to run this utility, kindly log in to your docker account.

#This will pull the image where the script is present
docker pull bhupender1988/movie_rating

#To check the images run the below command
docker images

#run the image as a container
docker run -ti -d [imagedid]

#Get the container id
docker ps

#Get inside container to execute script
docker exec -it [containerid] /bin/bash

#run the script , by passing movie name as an argument, note instead of python , we would be using command python3
python3 Imdb31.py Avengers

#expected output
Movie Name is ==>Avengers
Rotten Tomatoes Ratings -->92%

#Error Handled
Movie name not found
