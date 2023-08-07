Hello,

It`s my Postman and Git practise. I used free API website.

Here I used GET method to obtain all booked reservations.

![GET](https://i.imgur.com/LiI5xIG.png) - everything worked we got all reservations


Now I have to gather additional information like name, surname and some more which are essential to book reservation.
I picked ID:1098. 

![GET](https://i.imgur.com/1lVCAKV.png) - perfect, that`s what I needed 


In meantime I want to see if POST method is working correctly.
I copied necessary information in to "Body" section, choosen "raw" form and choosen "JSON" language.
Why? Because I received it in JSON and also as a respond want it in JSON.

![POST](https://i.imgur.com/pvqiRqA.png) - got 200 OK status so it`s working


Lets move in to another step. In documentation I see PUT and DELETE method are need authorization token.
Which means I have to create one using POST method and data from documentation.

![POST](https://i.imgur.com/aO8mg2H.png) - again all is good, but what I did here?
In body section pasted logins from docs written in JSON, sent to the server and as a respond I got token.
Every single time when I click send I get another token which have to update and use in remaining methods.


Now I have all to test the rest. I have mentioned I picked ID:1098 from the beginning and I am going to use this one now.

![PUT](https://i.imgur.com/WazcNk6.png) - seems It worked
Here I changed some values like name, surname, price and the rest and what is more important I had to use authorization token
which I have received from previous step. I implemented it in Headers like Cookie and value - token. 
Without this I wouldn`t be able to PUT or DELETE


Let`s see if really my choosen ID has been changed correctly. I have to pick GET method and use ID:1098

![GET](https://i.imgur.com/SrAFy7U.png) - awesome! This is what I wanted

Ok, last step and my TC is DELETE. Again I use ID:1098 to see if this method is working

![DELETE](https://i.imgur.com/9AU5oG5.png) - ok well, my record has been deleted. 

I am going to check it out by using GET method again

![GET](https://i.imgur.com/GpeTuCM.png) - Perfect



Results? API is working perfectly 





