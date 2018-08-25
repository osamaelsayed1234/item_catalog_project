# :octocat: ITEM_CATALOG :volcano::partly_sunny:
a full website:milky_way: with JSON API using Oauth2 provider for authentication with authorized users:rocket:.

## Used Technology:hammer:
* FLASK Framework:statue_of_liberty:
* Oauth2 provider:rainbow:
* SQLAlchemy:airplane:
# SETUP :fuelpump:
* first:pushpin: you need to download this project using the command: 
```
git clone https://github.com/hazemkhaledmohamed/ITEM_CATALOG 
```
* then run **Database_Setup.py** to initialize the database with null values with name **ItemsCatalogWithUsers.db**:umbrella:
* after that you need to write some data to the Data-Base file to test this app so run **Fake_Items.py**:ring:
* then run **APP.py**:full_moon: to run the server with home address **https://localhost:5000** with port 5000

# files contained in the project:seedling:
* ## **APP.py**:full_moon: 
this file contains tha whole app along with initializing the server 
this file contain the implementation of many features:gift: in the app such as CRUD functionality:palm_tree: (crate, Read, Update, Delete) elements form database with SQLAlchemy(ORM) package with python also this file contain decorator pattern:ear_of_rice: for each Url functionality such as this one for home page ```https://localhost:5000/```:mortar_board: also this file call the template files along with our project while running:tada: and render it's content to user Browser then this file implement the authentication :lock:for user want to connect to our app and specify authority:key: for each user according to his items which will enable him to add his own item and modify and delete it but not deleting other users items
,also this file has the API endpoint:electric_plug: which call the user's items in JSON form to allow other services or Developpers to build their app based on this API:bath:.

* ## **Fake_Items.py**:waning_gibbous_moon: 
this file initialize the database with some data to load to the server

* ## **Database_Setup.py**:last_quarter_moon: 
this file initializes:syringe: the data base tables and couloums with it's names and relations:scroll: which has the properties of serializing data to JSON format to be loaded to API endpoint:mailbox_closed:. 

* ## **ca.crt**:waning_crescent_moon: 
certificate file to install Https with the server:lock_with_ink_pen: with **ssl_context** attribute this specify both files the ca.crt and the ca.key which include the certificate and key for the server to communicate with client via Https request also this file is generated via OpenSSL.

* ## **ca.key**:new_moon: 
key file for certificate installation:closed_lock_with_key:,this file is generated via OpenSSL.

**notice**
here we use these two files to install certificate for our website in order to be used with 3rd party Oauth to authenticate facebook users via a secured **https** request
* ## **client_secrets.json**:earth_asia: 
Json file for google authentication with users in order to get token for each user while the server is running:trumpet:.

* ## **fb_client_secrets.json**:milky_way: 
Json file for google authentication:saxophone:.

* ## **ItemsCatalogWithUsers.db**
this file shouldn't be here:bookmark: but for testing your code without any misterious problems you can use it as is.

* ## **static**:skull:
this folder contain the styles.css file which has the styles for each component on the page also has the buttons style:snake: contained for each button in the website.

* ## **template**:zap:
this folder contain all website templates that loaded into python code for render it's data contined with appropriate URI entered:trollface:.
