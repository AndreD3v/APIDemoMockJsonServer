# Api Mock (running json-server)

Demo project using json-server (for more info see :: https://github.com/typicode/json-server).

## Description

Do you want a different API to test than the common used Petstore, for experimenting with your test tools? Here you have one :-) You can run it locally! 
And above all you can adjust it easilly. Add you own endpoints and own data easily.

Besides using this api for testing your testing tools, you can use it ofcourse as well for mocking your complex test situations (just adjusting the endpoints and data).

## Installation

- Clone this GIT folder to your local machine;
- install json-server with the following cmd comands :: npm install -g json-server
- Run powershell script 'LaunchAPImock.ps1' (non-primair mouseclick > Run with Powershell)

Note :: the API service can be killed with [CTRL] + [C].

## Run (local)

1. Run powershell script 'LaunchAPImock.ps1' (non-primair mouseclick > Run with Powershell)
1. The Powershell script does return the initial endpoints wich are curently available.
1. e.g. http://localhost:3000/sportscategories if you use this in its own you will get back all data available, but of course you can use the query parameters to make a sub selection

A few simple examples :: 

- http://localhost:3000/sportscategories?category=Water (search based on category label)
- http://localhost:3000/sports/1 (search based on id label)
- http://localhost:3000/sports?id=1&id=2 (search based on combining id labels)

## Add your own endpoints and data

1. Kill the runing server with [CTRL] + [C].
1. Open the db.json file
1. If you have played with the above examples you probably will recognize the structure of this file fast. 
1. just add a new endpoint by adding a new key-value pair at the same level as all other endpoints. 
1. Save the adjusted file and run again the powershell script.