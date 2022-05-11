# REST API

AtroCore is an API-centric application, so a frontend uses REST API to connect with a backend. Our REST API is based on OpenAPI (Swagger), so you can [generate your client](https://openapi-generator.tech/docs/generators/) automatically.

All operations you perform using UI can be performed via API requests using the programing language of your choice. 
You can learn how API works if you trace what's going in the network tab in your **browser console** (press F12 key to open the console).

All requests needs to have the header: `Content-Type: application/json`. 

The path to the API in AtroCore is: `/api/v1/`. Only this path can be used for your API requests.

> We recommend to create a **separate API user** with specific rights (configure and assign a role to him) and use this user for API calls.

## REST API documentation
REST API documentation is generated for each project automatically, based on your configurations and modules you are using. 

To access it please go to `https://address_of_your_atrocore/apidocs/`.

For example the documentation for demo.atropim.com is available here: [https://demo.atropim.com/apidocs/](https://demo.atropim.com/apidocs/)

## 1. Step: Authentication

To be able to use AtroCore API you need to go through authentication and obtain access token. Please watch the [video tutorial](https://youtu.be/GWfNRvCswXg) to learn how to authorize in the REST API.

For obtaining access token you need to send GET request to `/api/v1/App/user` using [Basic Authentication](http://en.wikipedia.org/wiki/Basic_access_authentication). 

## 2. Step: Making requests

To see which requests are available read the documentation for your AtroCore instance. 

To access it please go to `https://address_of_your_atrocore/apidocs/`.

Example of GET API request: 

```
GET https://address_of_your_atrocore/api/v1/Product/2d643ca0gff7rh7c6
```
## Video Tutorials
* [How to authorize?](https://youtu.be/GWfNRvCswXg)
* [How to select specific fields?](https://youtu.be/i7o0aENuyuY)
* [How to filter data records?](https://youtu.be/irgWkN4wlkM)




