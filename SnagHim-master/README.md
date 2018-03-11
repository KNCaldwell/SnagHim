# SnagHim

STEP # 1: 

    npm init

STEP # 2: 
    npm install body-parser@1.15.2"
    npm install cookie-parser1.4.3
    npm install debug@2.2.0
    npm install dotenv@5.0.1
    npm install express@4.14.1
    npm install hbs@4.0.1
    npm install morgan@1.7.0
    npm install mysql@2.15.0
    npm install serve-favicon@2.3.2
    npm install babel
    npm install webpack 
    npm install hbs-utils (will help you watch for changes in your partials 9and update them without having to restart the app)
    npm install express-validator
    npm install bcrypt
    npm install express-session
    npm install express-mysql-session --save
    npm install passport-local



STEP # 3:  
    npm install nodemon 

STEP # 4: 
    To run file run 'nodmeon .' 

STEP #5: 
    create a .env file in your Root Directory
    for Windows: add this to .env file
        NODE_ENV=DEVELOPMENT

            DB_HOST=127.0.0.1
            DB_USER=root
            DB_PASSWORD=  your password  
            DB_NAME=final_app
    for MAC: add these codes to .env file
        NODE_ENV=DEVELOPMENT

            DB_HOST=127.0.0.1
            DB_USER=root
            DB_PASSWORD=   
            DB_NAME=final_app
            socketPath: your path

            run a command netstat -ln | grep mysql| 
            copy the path in your socket pach above. 

STEP # 5:
    copy all schema.sql code in your sqlWorkbench to create database:


STEP # 6:
    setup the database migration to ensure that you are not directly interacting with you mysql. in this app

STEP # 7: add those following codes to mysql workbence 
        ALTER TABLE `final_app`.`users` 
        CHANGE COLUMN `username` `username` VARCHAR(15) NOT NULL ,
        CHANGE COLUMN `email` `email` VARCHAR(100) NOT NULL ,
        CHANGE COLUMN `password` `password` BINARY(60) NOT NULL ,
        ADD UNIQUE INDEX `username_UNIQUE` (`username` ASC),
        ADD UNIQUE INDEX `password_UNIQUE` (`password` ASC);


