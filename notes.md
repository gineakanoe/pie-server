
npm - Node Package Manager

    npm init -y    
                - initialize on server      - creates package.json file 

    npm start      
                - looks into root directory; looks for scripts of object; looks for mathching keyword (aka 'start' in this case); runs command script

    npm dev (aka development)   
                - indicates project is running in development mode, and we're using 'nodemon' to do that.
                Nodemon - allows us to make changes to server w/o having to restart it manually every tume we make a change.

    npm install --save-dev nodemon
                - creates node_modules folder & package-lock.json
                    - node_modules: packages npm installs that all our application and all its dependencies to run properly
                    - package-lock.json: locks in the version of packages we're using in project.  IF project is CLONED and run, it will have the exact same versions of packages.

    npm install express
                - adds Express to project
                        - a framework used to organize server into MVC architecture
                            - MVC: Model View Controller
                                    -Models: how we shape the data that is sent to the databases. 

                            - ORM: Object Relational Mapper
                                    - Code library that automates transfer of data in database into objects that are more commonly used in application (like JSON)


    npm run dev

        Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass

    npm install dotenv 
                - environment


Note: ctrl + c will stop any running server in terminal


    npm install sequelize
                - Sequelize: a JS library that is used to manage postgreSQL database.

    npm install pg pg-hstore
                - pg: a package taht lets us write in a dialect sequelize needs to speak to PostgreSQL database.
                - pg-hstore: package that lets us access more advanced & complex pieces of code regarding PostgreSQL.

    npm install chalk



Instructor Notes:

npm- Node package Manager, can manage packages that are local dependencies of a particular project.

npm start - this command looks into the root directory of our project, and looks for the scripts object. If it finds it, it will look for the matching keyword(in this case, it's "start") then runs the following command script

npm dev - Indicates that we are running our project in development mode and that we are using 'nodemon' to do that. Nodemon allows us to make changes to our server without having to restart it manually every time we make a change

node_modules - packages that npm installs that allow our application and all of its dependencies to run properly

package-lock.json - simply locks in the version of the packages that we're using in a specific project. We get this file so that anyone who clones our project and tries to run it will have the exact same versions of the packages that we use.

MVC - Model View Controller

Models - how we shape the data that we'll be sending to our databases

Express - a framework used to help us organize our server into MVC architecture.

ORM - Object Relational Mapper. Code library that automates the transfer of data in a database, into objects that are more commonly used in applications(like JSON)

Sequelize - a JS library that we'll use to manage our postgreSQL databases.

pg - a package that allows us to write in the dialect that sequelize needs to speak to our PostgreSQL database

pg-hstore - a package that allows us to access more advanced and complex pieces of code regarding PostgreSQL

pgAdmin - is a GUI (Graphic User Interface, pretty much a front-end client) that allows us to visualize our PostgreSQL database. pgAdmin is one of many GUIs that interface with PostgreSQL.

pgAdmin and PostgreSQL are not the same thing. PostgreSQL is a database engine implementing SQL standards.

pgAdmin is a sort of client. You are able to manipulate schema and data on an instance or multiple instances of PostgreSQL engines.

bcrypt - used to encrpt sensitive data such as user passwords

jwt - used to create sessions