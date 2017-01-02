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

Now there are 2 micro-services registered on registration service.
![Killed account02](images/account_second04.png)

The registration service can't provide information about account service on port 2222 because there's no connection so,
it can't be registered on the registration service.