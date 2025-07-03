## 🚀 Thankyou for this Amazing Tech Stack project by DevOps Shack 

# Userdetails App

This is a full-stack JavaScript application that manages user data using a React.js frontend and an Express.js backend, running on Node.js.

---

| Layer        | Technology     |
|--------------|----------------|
| Frontend     | React.js       |
| Backend      | Express.js     |
| Runtime Env  | Node.js        |
| Language     | JavaScript     |
| Init Tool    | npm (Node Package Manager) |

---

Step-1
Installing node.js in my Linux machine 
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 22

# Verify the Node.js version:
node -v # Should print "v22.17.0".
nvm current # Should print "v22.17.0".

# Verify npm version:
npm -v # Should print "10.9.2".


---
Step-2

## ⚙️ Installation & Setup process

### 1. Clone the Repository
```bash
git clone https://github.com/gowthamgandhari/Userdetails.git userdetails
cd Userdetails

step-3
--> sudo apt install mysql-server -y

--> ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'gowtham'; # u can keep ur-own passwd 
    FLUSH PRIVILEGES;
    EXIT;

--> sudo mysql -u root -p  # give ur passwd

--> CREATE DATABASE IF NOT EXISTS crud_app;

--> USE crud_app;

--> DROP TABLE IF EXISTS users;

--> -- Create the `users` table with proper structure

   CREATE TABLE IF NOT EXISTS users (
   id INT AUTO_INCREMENT PRIMARY KEY,
   name VARCHAR(255) NOT NULL,
   email VARCHAR(255) NOT NULL UNIQUE,
   password VARCHAR(255) NOT NULL,
   role ENUM('admin', 'viewer') NOT NULL DEFAULT 'viewer',
   is_active TINYINT(1) DEFAULT 1,
   created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP

step-4
open the 2 terminals 1 for client and 2 for api 

In ur Linux machine u cloned the repo rt  go to ur cloned directory :
--> git clone https://github.com/gowthamgandhari/Userdetails.git userdetails

--> cd userdetails
--> userdetails #/ cd api
--> api #/ vi .env
--> cat .env
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=Gowtham # u can replace ur passwd    
DB_NAME=crud_app
JWT_SECRET=devopsShackSuperSecretKey  # as well as this key also 

--> npm install  #it creates the node_modules folder here again 

--> npm start 

 here you can see that MySQL is Connected 


Step-5
In ur Linux machine u cloned the repo rt  go to ur cloned directory :
--> git clone https://github.com/gowthamgandhari/Userdetails.git userdetails
    cd Userdetails
    npm install

--> cd ../client in this folder u have .env file here  go and modify your pubip: REACT_APP_API=http://18.191.151.160:5000  and save it

--> npm install   # when u install it creates the node_modules directory 

--> cd src  # move to src folder to to execute the testcases give command 
 
--> npm test

--> npm start



Then run in browser: http://localhost:5000
