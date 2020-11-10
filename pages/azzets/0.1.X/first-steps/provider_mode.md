---
title: Provider Mode
permalink: /azzets_0.1.X_provider_mode.html
toc: false
---

***
## Create User  

First impression upon access.
Upon identifying ourselves, our main window will appear. A Provider user could only create other provider type users and the new users belong to the same Provider. To do this we click on `Administration / User Management`. 

{% include image.html file="azzets/createProviUser/creatNUserinit.png" alt="Create User" %}  

***

We click on the `+` symbol and fill in the fields of the Form that appear:  
{% include image.html file="azzets/createProviUser/formProvUser.png" alt="Create User" %}  

*Email*: It is the access user  

*First Name*: This is the name of the user who will use this account  

*Last Name*: This is the last name of the user who will use this account.  

*Wizzie Token API*: This is a Token API that Wizzie must give to the user. Without this API the user cannot work in the system, it is necessary to be able to load the Wizzie organizations and to be able to create Provider.  

*Language*: This is the user's preferred language. The application supports three languages, Spanish, English and Catalan  

***
At the end we click on the `SAVE` button and this will take us to the window where all the users created that belong to the same Provider will be, the application gives us the option to delete or modify a user if we wish:  

{% include image.html file="azzets/createProviUser/provUserEnd.png" alt="Create User" %}



***
## Create Azzets-Use (can only from your Provider)  

Before creating the Assets, we must create an Assets User, who is going to use the Assets that we will create later, for them we go to the `Entities / Assets User` tab:

{% include image.html file="azzets/CreateProviAzzetsUse/entitiesAzzUse.png" alt="Create User" %}  

***
We click on the `+` symbol and fill in the fields of the Form that appear:  

{% include image.html file="azzets/CreateProviAzzetsUse/formPUseAzz.png" alt="Create User" %}


*Identifier*: This is the name of the Azzets Use.  

*Description*: A brief description of the Azzets use.  
* * *


At the end we must click on the `SAVE` button, and this will take us to the window where all the Assets Use created will be, the application gives us the option to delete or modify an Assets Use if we wish:  

{% include image.html file="azzets/CreateProviAzzetsUse/endPUseAzz.png" alt="Create User" %}
* * *
## Create Azzets (you can only from your Provider)  

The Azzets is the one who sends the data to the kafka topics to create a new Assets, we go to the `Entities / Assets` tab:

{% include image.html file="azzets/CreateProviAzzets/entitiesAzzets.png" alt="Create Azzets" %}  

***
We click on the `+` symbol and fill in the fields of the Form that appear:  

{% include image.html file="azzets/CreateProviAzzets/formAzzp.png" alt="Form" %}
 
*Identifier*: This is the name of the Assets that we are creating.  

*Description*: A brief description of the Assets created.  

*Vendor*: It is an identifier.  

*Asset Use*: This is the list of all Azzets Use created, you must choose the one you are going to work with.  

The enable checkbox, we must mark it.  

***
At the end we must click on the `SAVE` button, and this will take us to the window where all the Assets created will be, the application gives us the option to delete or modify an Assets if we wish:  
{% include image.html file="azzets/CreateProviAzzets/provAzzEnd.png" alt="End" %}  

***

The application automatically sends the data to the kafka topic, as the events are created. It also gives us the option to forward the entire stream using the `Synchronize` button