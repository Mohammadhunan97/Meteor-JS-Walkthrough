

 Meteor-JS-Walkthrough
__________________________

Meteor JS is a NodeJs framework built to easily create apps using MVC Structure: 

Meteor JS uses websockets to have real time updates

Meteor uses live reloading so you don't have to refresh/restart your server everytime you make a change

Meteor uses collections to interact with database stuff on both the client and server easily and quickly



To install: 
  _______
  
  curl https://install.meteor.com/ | sh


Setup:
 ___
 
  meteor create myapp
  cd myapp
  meteor




Templating:
 ________
 
 Html is templated as such:
 
 <template name="welcomemsg">
     <h1>Hi, and welcome to our app </h1>   
 </template>
 
 Rendering the template: 
 
 {{> welcomemsg}}


to loop through data:

 {{#each x}}
   {{> y}}
 {{/each}}

client/main.js:
x is the array which holds all the objects you want to put inside the loop
y is how you want the data to be displayed as, you can define this in your template tag:

 <template name="y">
    <h1>{{key_inside_of_x_array}}</h1>
 </template>


To create a collection:
 ____________________
 Users = new Mongo.Collection('users');
 
 in terminal:
 meteor mongo
 


remove autopublish from packages because its insecure
