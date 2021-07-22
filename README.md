# DailyGate.com Websites


## Login Module


    In login module there are two login module company login and teammate login,
    let we discuss on teammate login module, which contain username or mobile along with correct password
    
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
  >this Ajax call for login messanger account to send messages related the task and discussion and Ajax call js file path is assets/js/app-bkp20jul.js and created js                 function name is loginMessengerAccount() and data is userEmail,userPassword passing email id in both data input and send method is POST and request url is                         messenger/registration/login/
           
  ### * Login Controller
  ##### 1) Authentication Controller of Function
  >this function is gets the username and password and passed it in signin_model get teamates data from database and created array passed it and gets company details using sign_id of teammate and passed it in created array and set session storage on browser and redirect dashboard view page and Controller path is application/controllers/associate/Signin.php in folder structure
  
  ### * Login Model
  >
