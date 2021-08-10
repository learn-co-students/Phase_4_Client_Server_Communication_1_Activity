# Phase_4_Client_Server_Communication_1_Activity

1. Create a new rails api called concert venues
2. Generate resources for Show and Ticket. 
A Show may have many tickets but a ticket will belong to a single show.   
```
Show -< Ticket 

***Show***  
date : datetime   
airtist : string  
all_ages : boolean.  

***Ticket***  
price : float   
show : belongs_to  
ticket_owner : string  
willcall : boolean 

```

3. Migrate

4. Add these seeds to seeds.rb and create your seeds
```
Show.create(date:DateTime.strptime("08/01/2021 16:00", "%m/%d/%Y %H:%M"),artist:'skrillex', all_ages:true)

Show.create(date:DateTime.strptime("08/15/2021 16:00", "%m/%d/%Y %H:%M"),artist:'daft punk', all_ages:true)

Show.create(date:DateTime.strptime("08/21/2021 16:00", "%m/%d/%Y %H:%M"),artist:'Drake', all_ages:true)


```

5. In route.rb limit your routes to include only the index

6. In the shows controller create an index action that will render all of the shows. 

7. run the server and go to `http://localhost:3000/shows` to confirm your data