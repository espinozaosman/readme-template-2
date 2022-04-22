**Description**
<br>
We have two APIs which use lambdas to process the tenant/app id. The two APIs are below:

1. `/contentful/broadcastsignal`
2. `/my-resources`

How to use `/contentful/broadcastsignal:`

This is a notification POST API that will send notifications to the user using OneSignal and return a response status code of 200. 
You will need to send the below keys in the header of the API:

1. Contentful-Key
2. Contentful-Token
3. Key
4. App-Id

In the request body, please use the below format:

`{sendNotification: boolean, id: string, title: string, subtitle: string, image: string, client: string}`

How to use `/my-resources:`

This is a GET API request that will provide the home page information in response.



