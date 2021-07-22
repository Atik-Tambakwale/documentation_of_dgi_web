# DailyGate.com Websites


## Login Module


In login module there are two login module company login and teammate login,let we discuss on teammate login module, which contain 
username or mobile along with correct password
    
 * login ajax Call
 * login controller
 * login model
 * login view
    
  ### * Login Ajax call
  there are two ajax call one for login authentication and another for messager connect the messager connect with dailygate website 
  
  ##### 1) Authentication Ajax call
  >this Ajax call for authentication of login done by username and password which given in Sign in view page and ajax call js file path is assets/js/app-bkp20jul.js
  which is submit eventlistener on login button id which is name "associate-login-frm"  and url is associate/signin/authenticate and data is email,password and token in             cookie and send method is POST method.
            
  ##### 2) Messanger Ajax call
  >this Ajax call for login messanger account to send messages related the task and discussion and Ajax call js file path is assets/js/app-bkp20jul.js and created js                 function name is loginMessengerAccount() and data is userEmail,userPassword passing email id in both data input and send method is POST and request url is                         messenger/registration/login/ and this ajax call work only on website server. 
           
  ### * Login Controller
  
  >this function is gets the username and password and passed it in signin_model get teamates data from database and created array passed it and gets company details using sign_id of teammate and passed it in created array and set session storage on browser and redirect dashboard view page and Controller path is application/controllers/associate/Signin.php in folder structure
  
  ### * Login Model
  >this Model Class contain auth() function to provided teammate all details using user_id and password and first we get teammate data from database after that verifying the password  and creates an array gets teammate and database connection details and check teammate is delete or not after return that array to controller it model function is call.  
  ### * Login View
  >this view provided  for user can enter the username and password and view file path is application/views/home.php
