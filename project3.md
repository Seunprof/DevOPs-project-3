# Documentation of project 3
### In this project, i learnt about other Web Stack Implementation used in AWS.
### In this project, i learnt and worked with LEMP (Linux, Nginx, MySQl, PHP) WEB STACK.
### This project was done using the steps below:
#### 1. Setup AWS account and Provisioned an Ubuntu Server
### 2. Created an EC2 Instance and Connected to the EC2 Instance
- Got the SSH link of the Instance

![SSH link](./images\ssh-connect.PNG)

-Pasted the SSH link to  the terminal and connectted to the instance

![SSH connect](./images\ssh.PNG)

### 3. Backend Configuration
### - Updated and upgraded ubuntu using the following commands repectively:
`sudo apt update`

`sudo apt upgrade`
### - Installed Node.js with the command below
`sudo apt-get install -y nodejs`

### - Verified the node installation with the commands below:
`node -v` 
![node version](./images\node-version.PNG)

`npm -v`
![npm version](./images\npm-version.PNG)

### - Created a new directory for your To-Do project:
`mkdir Todo`

### - Changed the current directory to the newly created one:
`cd Todo`
### -  Initialise the project, so that a new file named *package.json* was be created. This was done by runnig:
`npm init`
![npm init](./images\npm-init.PNG)

### The file *package.json* is shown below:
![Package json](./images\json.PNG)

### 4. Install ExpressJS
### - Express was installed using npm:
`npm install express`

### -  Created a file *index.js* with the command below
`touch index.js`

### - Installed the dotenv module
`npm install dotenv`

### - Opened the index.js file with the command below
`vim index.js`

### - Typed the code in the file as shown below into and saved.
![Index script](./images\index-code.PNG)

### - Checked to see that the server worked by running the code:
`node index.js`

### The picture as shown below revealed that the server worked
![Server](./images\server-port.PNG)

### - Opened the EC2 Security Groups, added a new inbound rule for TCP port 5000 as shown below:
![TCP port](./images\tcp-port.PNG)

### The picture below revealed the site from Express perspective.
![Express](./images\express.PNG)

### 5. Creation of task for To-do application
### For each task, we need to create routes that will define various endpoints that the To-do app will depend on. 
### - Firstly **routes** folder was created using the code:
`mkdir routes`

### - Changed directory to routes folder.
`cd routes`
### -  Created a file *api.js* with the command below
`touch api.js`
### - Opened the file with the command below
`vim api.js`
### - Pasted the codes as shown below into the file and then save:
![api](./images\api-ls.PNG)

### 6. Create a Schema and a model

### A model is at the heart of JavaScript based applications, and it is what makes it interactive.

### - Changed directory back Todo folder and installed Mongoose using the code:
`npm install mongoose`

### - Created a new folder models :
`mkdir models`

### - Changed directory into the newly created ‘models’ folder and created a file *todo.js* inside the file
`touch todo.js`

### - Opened the *todo.js* file and pasted the codes as shown below into it, then saved:
![model](./images\model-todo.PNG)

### - Opened the *api.js* file in the **Route** directory and pasted the codes are shown below, and then saved
![New api](./images\new-api.PNG)

### MongoDB Database: A database where data will be stored is needed. For this purpose mLab was used. mLab provides MongoDB database as a service solution (DBaaS).
