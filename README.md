

# Meteor-JS-Walkthrough

Meteor JS is a NodeJs framework built to easily create apps using MVC Structure: 

Meteor JS uses websockets to have real time updates

Meteor uses live reloading so you don't have to refresh/restart your server everytime you make a change

To install: 

  curl https://install.meteor.com/ | sh


Setup:

  meteor create myapp
  cd myapp
  meteor
  
 Templating:
 
 Html is templated as such:
 
 template name="welcomemsg"
 
     Hi, and welcome to our app
     
 /template
 
 Rendering the template: 
 
 {{> welcomemsg}}
