# nana-tutorial-docker
This is adocker handson ttutorial repo followed by watching nana janashia on youtube 
https://www.youtube.com/watch?v=3c-iBn73dDE
https://gitlab.com/nanuchi/techworld-js-docker-demo-app  these are her youtube video and repo link
'to run this project you need to have configures docker in your systenm this project repo is based on windows system'

to run this docker application 
you need to do following changes in server.js file on line 25
let mongoUrlLocal = "mongodb://admin:password@mongodb:27017"; 

and run these commands
to start mongo and mongo express
  
  docker-compose -f docker-commands.yaml up

and then go to localhost:8080 and create a database named my-db and collection named users

to run the node server app container 

  docker build -t my-app:1.0 . 
  docker run -p 3000:3000 --net docker_default my-app:1.0
  
and then you can use your nodejs application in on localhost:30000
#goodluck 
#ThanksTechWorldwithNana
