TodoApp - Here data will store in databse (Firebase is the database we used)
An app that stores the list of activities you make to do. 
The funtionalities of the sampletodo are : 
	adding todo 
	removing todo 
	updating todo(editing todo)
	toggling todo 
	toggling list of todos 
	filtering 
	clearing completed todos


**************************************************************************************************************************************************************************************************************

                                                                                   HOW TO WORK WITH OUR PROJECT:

1 . Git Cloning :
    
    

2. Navigate to our project folder

3. There you will find dscript.sh file

   open terminal there and run script using sh dscript.sh

   This script contains :

   * docker image build -t myimage . (Create docker image from docker file)
   * docker container run --publish 3006:3000 --detach myimage (This will run image to get container and mapped the container port to host port)
   
   
4.Goto browser :

	Browse for :

	
	http://localhost:3006/ 


*************************************************************************************************************************************************************************************************************

                                                                                   Ansible Output

ashu@ashu-HP-Laptop-15q-ds0xxx:/etc/ansible$ ansible-playbook todoappplay.yml
[DEPRECATION WARNING]: The TRANSFORM_INVALID_GROUP_CHARS settings is set to allow bad characters in group names by default, this will change, but still be user configurable on deprecation. This feature 
will be removed in version 2.10. Deprecation warnings can be disabled by setting deprecation_warnings=False in ansible.cfg.
[WARNING]: Invalid characters were found in group names but not replaced, use -vvvv to see details


PLAY [ap-south-1] ******************************************************************************************************************************************************************************************

TASK [Gathering Facts] *************************************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Install git] *****************************************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Install aptitude using apt] **************************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Install required system packages] ********************************************************************************************************************************************************************
ok: [13.232.233.38] => (item=apt-transport-https)
ok: [13.232.233.38] => (item=ca-certificates)
ok: [13.232.233.38] => (item=curl)
ok: [13.232.233.38] => (item=software-properties-common)
ok: [13.232.233.38] => (item=python3-pip)
ok: [13.232.233.38] => (item=virtualenv)
ok: [13.232.233.38] => (item=python3-setuptools)

TASK [Add Docker GPG apt Key] ******************************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Add Docker Repository] *******************************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Update apt and install docker-ce] ********************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Install Docker Module for Python] ********************************************************************************************************************************************************************
ok: [13.232.233.38]

TASK [Execute the script] **********************************************************************************************************************************************************************************
[WARNING]: Consider using 'become', 'become_method', and 'become_user' rather than running sudo

changed: [13.232.233.38]

PLAY RECAP *************************************************************************************************************************************************************************************************
13.232.233.38              : ok=9    changed=1    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

*************************************************************************************************************************************************************************************************************


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
   
    
    
