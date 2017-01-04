# Registration Service
Registration service started.
![Registration started](images/registration.png)

![Registration started02](images/registration02.png)

#Account Service
Account service started on port 2222.
![Account service](images/account.png)

![Account service02](images/account02.png)

#Web Service
Web service started on port 3333.
![Web service](images/web.png)

The two services are registered on the registration micro-service.
![Web service02](images/web02.png)

#Second account service
A new account service is started on port 4444.
![Second account service](images/account_second.png)

The three services are registered on the registration micro-service.
![Second accounr service02](images/account_second02.png)

#Killing account service
The account service on port 2222 is killed.
![Killed account](images/account_second03.png)

Now, when the web service tries to communicate with the account service on port 2222, it gets a connection refused. Then, the web service communicates with Eureka asking for an account service, Eureka gives to it the account service on port 4444 and the web service can work again.

One account service.
![Killed account02](images/account_second04.png)

The web service keeps working thanks to Eureka.
![Killed account03](images/account_second05.png)