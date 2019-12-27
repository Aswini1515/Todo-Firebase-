## TodoApp 
An app that stores the list of activities you make to do. 

## Tech stack
1. ReactJs - Frontend
2. Firebase - Database

#### The application is responsible for: 
	1. Adding todo 
	2. Delete todo 
	3. Updating todo
	4. Toggling todo 
	5. Toggling list of todos 
	6. Filtering 
	7. Clearing completed todos

## Developers Guide

* npm create-react-app appname


* npm install (npm install should be done , to run npm start)
* npm start

Firebase:

npm install firebase --save


npm install string 




Docker:

* Create docker file with required dependencies (touch dockerfile)

* Building docker file:
    To make the image need to use this command-->sudo docker image build -t "name of your choice"(quotes not required and . required) .
    after some time image will be created.
    *To check whether the image is formed or not need to run following command-->sudo docker run -it react bash
        then we can observe container id and path .. if we want to check the files give ls command and can find node_modules,src,public,
        package.json
        we can check by start npm then we get ip's
        -->npm run build command ,, in main container then will sasee 
        exit and come back to main project in command line and write
        sudo docker cp (container id):/usr/src/app .  , to get whole container data into our server including with build
   
    
    
