---
title: Root Mode
permalink: /azzets_0.1.X_root_mode.html
toc: false
---
* * *
First impression upon access.
When we identify ourselves, our main screen will appear, where the first thing we will do is manage our account. We click on `Administration/User Management`

{% include image.html file="azzets/useRoot/cnu_manager1.png" alt="Create User" %}

* * *
Here we see our user and we click on edit, we get a new window where we will fill in the form.

{% include image.html file="azzets/useRoot/formRoot.png" alt="Form" %}

*Username "email"*: It is the login user

*First Name*: This is the name of the user who will use this account eg. Robert

*Last Name*: This is the Surname of the user who will use this account. ex. Smith

*Wizzie Token API:* This is an API Token that Wizzie must give to the user. Without this API the user cannot work in the system, it is necessary to be able to load the Wizzie organizations and to be able to create Provider

*Language:* This is the user's preferred language. The application supports three languages, Spanish, English and Catalan


* * * 
   {% include image.html file="azzets/useRoot/enduser.png" alt="End" %}             
_ _ _
There are two types of users, root and a Provider administrator:

1- Root:

The root and activated check boxes are marked by default, to create a root user we must select both check boxes. If you are root, you will have access to all the Providers and all the information.
At the end we click on the blue `SAVE` button.

{% include image.html file="azzets/createUserRoot/checkboxroot.png" alt="Create User" %}

2- Provider:  
In the event that the user we are creating is not root, we must uncheck the root checkbox and specify the Provider to which it belongs. This user will only see the data of their Provider.

{% include image.html file="azzets/createUserRootProvider/user-noroot.png" alt="Create User" %}

* * *
## Create a Provider  

Once the user's data is updated, we must create a new provider, for this we go to the `Entities / Provider` tab:
 

{% include image.html file="azzets/crateRootProv/enntitiesProvider.png" alt="Create User" %}

* * *
We click on the blue `Create A New Provider` button and fill in the fields of the Form:

{% include image.html file="azzets/crateRootProv/formProvider.png" alt="Create User" %}  


*Identifier*: This is the name of the provider we are creating.  

*Description*: A brief description of the provider  

*Topic*: This is the name of the topic to which you are going to subscribe  

*Wizzie Organization*: Wizzie Organization to which you are sending the data. In this case there are three organizations available (FIRA, ITNOW, UCLM), the user must choose one.

* * * 

At the end we must click on the blue SAVE button, and this will take us to the window where all the providers created will be, the application gives us the option to delete or modify a provider if we wish:

   {% include image.html file="azzets/crateRootProv/providerEnd.png" alt="Create User" %}             
_ _ _

***
## Create An Azzets Use
Before creating the Assets, we must create an Assets User, who is going to use the Assets that we will create later, for them we go to the  `Entities / Assets User` tab:

{% include image.html file="azzets/createRootazzetsUse/entitiesAzzUse.png" alt="Create User" %}  

***
We click on the blue `Create A New Azzets Use` button and fill in the fields of the Form:  

{% include image.html file="azzets/createRootazzetsUse/formAzzUse.png" alt="Create User" %}  

*Identifier:* This is the name of the Azzets Use.  

*Description:* A brief description of the Azzets use.  

*Provider:* This is the name of the Provider you are using. The application shows us the list of Providers that are created, the user must choose between them.  

***

At the end we must click on the blue `SAVE` button, and this will take us to the window where all the Assets Use created will be, the application gives us the option to delete or modify an Assets Use if we wish:  
{% include image.html file="azzets/createRootazzetsUse/AzzUseEnd.png" alt="Create User" %} 

* * *
## Create an Azzets
 
The Azzets is the one who sends the data to the kafka topics. To create a new Assets we go to the `Entities / Assets` tab:  


{% include image.html file="azzets/createRootazzets/entitiesAzzets.png" alt="Create User" %}

* * *

We click on the blue `Create A New Azzets` button and fill in the fields of the Form:  

{% include image.html file="azzets/createRootazzets/formAzzets.png" alt="Create User" %}  
_ _ _
*Identifier*: This is the name of the Assets that we are creating.  

*Description*: A brief description of the Assets created.  

*Vendor*: It is an identifier.  

*Provider*: This is the list of all the Providers created, you must choose the one to work with.  

The enable checkbox, we must mark it.  

* * * 
At the end we must click on the blue SAVE button, and this will take us to the window where all the Assets created will be, the application gives us the option to delete or modify an Assets if we wish:  

{% include image.html file="azzets/createRootazzets/createAzzetsEnd.png" alt="Create User" %}  

          


The application automatically sends the data to the kafka topic, as the events are created. It also gives us the option to forward the entire stream using the Send Kafka button.