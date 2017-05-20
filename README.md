# ts3api
A NODE server that connects to your local Ts3 instance for easy communication via api with php or other languages.


Please create a config.json file in the root folder
fill out the following example and copy it into the config.json

config.json example:
```json
{
    "server":{
        "loginname": "< query login name >",
        "loginpw" : "< login password for your query >",  
        "apiport" : "< the port, your api is available at localhost >",
        "socport" : "< socket port for the ts3 query login, default is: 10011 >",
        "sochost" : "< socket host, normally its 127.0.0.1 >",
        "apiaccess" : "< access type to the api, if set to 'local' access is granted to localhost only >", 
        "nickname" : "< name of the bot >",
        "sid" : "< virtual ts3 server id, normally its 1 >"
    },
    
    "local":{
        "loginname": "< query login name >", 
        "loginpw" : "< login password for your query >", 
        "apiport" : "< the port, your api is available at localhost >",
        "socport" : "< socket port for the ts3 query login, default is: 10011 >",
        "sochost" : "< socket host, normally its 127.0.0.1 >",
        "apiaccess" : "< access type to the api, if set to 'local' access is granted to localhost only >", 
        "nickname" : "< name of the bot >",
        "sid" : "< virtual ts3 server id, normally its 1 >"
    }
}
```
the server subcategory is for production use on your server
the local subcategory is for development on your local system

start the server by running:
npm run dev
for development and
npm run prod
for running in a production environment