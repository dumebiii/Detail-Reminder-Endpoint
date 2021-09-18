# Zuri Chat Core API (Calendar plugin ) (1.0.0)
Zuri Chat is an open source slack clone. However, it offers a lot more functionality via a plugin system where each room can be provided by a different plugin provider.






# REMINDER:DETAIL
### Description: Get details of a particular reminder
```sh
PATH PARAMETERS: reminder_id(required)
```



## How it works
####  It works when there is a ( get  request)made to a particular reminder_id to get details of the reminder linked to the reminder_id.

### HOW TO SET UP THE END POINT

These are ways to set up the end point to function properly:

- With the help of python set up django framework
- Create all necessary files like ( url.py  ,serializer.py, views.py)
- Import all needed modules
- It is important you set your database up with models.py
- Copy the URL for the reminder get request
-   ‘GET’\https://calender.zuri.chat/api/v1/reminder_detail/reminder_id
- Paste it where it is needed in the code which is  the url.py 
That is a summary of how the end point is being set up.


#### STEPS ON HOW TO USE 
- We must make sure we have a reminder_id (to trace the particular reminder)
-  We then use the URL 
https://calender.zuri.chat/api/v1/reminder_detail/reminder_id
- We would receive a response message, you can see below list of different  responses

### RESPONSES;
#### 200          
#### Successful

```sh
{
  "status": 200,
  "message": "string",
  "data": string
}

```


#### 404
#### The reminder is not found on the database

```sh
{
  "status": 404,
  "message": "string",
  "data": null
}

```
