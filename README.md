INTRODUCTION
------------
The To-Do List allows the user to enter lists and assign tasks. The tasks are ordered by due date.

REQUIREMENTS
------------
Ruby v 2.2.0
postgreSQL 9.4.0


INSTALLATION
------------
Run the following command to install pg:
  `gem install pg`

Run the following command to run the postgreSQL server:
  `psql`

Run the following commands to create the databases:
  `CREATE DATABASE to_do`
  `\c to_do`
  `CREATE TABLE lists (id serial PRIMARY KEY, name varchar)`
  `CREATE TABLE tasks (id serial PRIMARY KEY, description varchar, list_id int);`
  `CREATE DATABASE to_do_test WITH TEMPLATE to_do; `

Run the following command to install bundle:
  `gem install bundle`

Run the following command to install all required gems:
  `bundle`

Run the following command to install rspec:
  `gem install rspec`

KNOWN BUGS
---------
Errors out when incorrect date format is entered.

AUTHOR
-------
Lauren Marcus
lauren.e.marcus@gmail.com

Amy Michelle Johnson
amy.johnson.michelle@gmail.com


LICENSE
-------

Copyright (c) 2015 Lauren Marcus & Amy Michelle Johnson

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
