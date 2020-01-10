# X5-FAIR-EzTalk
This file explains the problem statement, proposed solution and all the other details required to familiarise with the project idea.

## Contributors
This Project is made by Yangtao Ge([YangtaoGe518](https://github.com/YangtaoGe518)), ChoiLam Wong([WongChoiLam](https://github.com/WongChoiLam)) and ([Zekun-Yang](https://github.com/Zekun-Yang))

Here is the detail responsibilities:
* *Yangtao Ge* is the team leader and the coordinator of the project; He also take responsibilities for front-end developing and project deployment.
* *ChoLiam Wong* is the back-end developer who takes charge of server side for processing the API with Data; He also maintains the project document as well as API document.
* *ZeKun Yang* is the front-end developer who responses for implementing individual components.

## Problem Statement
Our topic is **Refugee Integration and Digital Education, Literacy & Refugee Children**

Europe has recieved a large influx of refugees in recent years. Refugees arrived are often not familiar with the language used in their destination, which stops them from finding a job, getting education for their offsprings and contributing to society. We identified two major barriers preventing them from learning the language which are the lacking of education materials and isolation of community. We aimed to support refugees by removing the barriers listed above.

* **Lacking of Education Materials** : Refugees don't often have access to suitable OERs. Either the materials are not written in their language or not written for their level of competence.
* **Isolation of community** : Often, refugee families find it easiest to isolate themselves in small communities in order to cope with new and unfamiliar environment. Their attempts to connect with others are inhibited by deficient English ability. As a result, they remain isolated and cannot improve their language skill by communicating.

## Proposed Solution
In order to solve the problems we stated above, we decided to develop a website pwa app called **EzTalk**, which is an app for language learning and socializing.

This app has these following key features:
* Provide OERs related to language studying
* Provide personalized recommendation of materials to each user
* Customized translation according to situation
* Chatroom for people to connect

In addition, we decide to develop a PWA(Progressive Web App) which is basically mobile-app-like website. It allows user can access the app by **only a url link** without downloading any apps.
This achieve our target of using convenience.

**X5GON's API** is used to retrive materials from x5gon, analysis material and translate;

## Project Structure
This project is collaborated on github orgnization([ROJHackathon](https://github.com/ROJHackathon)), all repositories are avaliable by this orgnization link.

* [Back-End-EzTalk](https://github.com/ROJHackathon/Back-end-EzTalk):
     This server is developd on **Java Spring Boot**, which provides the API service for front-end app to use. The backend server is deployed on a *private server* on *http://108.61.221.218:39802*. 
* [Front-End-EzTalk](https://github.com/ROJHackathon/Front-end-EzTalk):
    The user interface is developed on **React.js & Framework7**, which display the PWA in a *IOS* style layout.
* [Documents](https://github.com/ROJHackathon/Documents):
    Documents folder includes the general plan of developing.
* [API-Document](https://github.com/ROJHackathon/API-Documents):
    It is possinle API avaliable from the backend; Noticed that X5GON's APIs are encapuslated from the backend server, which can automatically analysis in backend.

![Structure](/assets/structure.png)

### Users
the users can access the website using any browsers with a URL
### Eztalk
eztalk manages all the material retrieved from x5gon and recommend materials based on machine learning algorithm




## How to Deploy 
Since we have two parts -- Front-end and Back-end, we will discuss they individually:
### Back-end:
Here are two ways to run the server:
* **Directly access the website** (Recommended): You can refer to the [API-Document](https://github.com/ROJHackathon/API-Documents) to get any avaliable APIs on *[https://ez-talk-api-provider.azurewebsites.net](https://ez-talk-api-provider.azurewebsites.net)* 
* **Deploy on your own**: on local machine run `mvn clean package` to deploy the server. Then run `mvn spring-boot:run` to run the server `localhost:8080`

Although it is possible to run on your local machine, we *do not* recommended to do so.

### Front-end:
Unlike server, you can run the clinet app on your local machine and it is recommended. 

To build the project: `npm i` and run `npm start` to run the server. 

Since it is a PWA, we recommend to use *mobile mode* to view the project to get a better perspective, to do so:
* You may use **Google Chrome** to access developer tool.
* Change to any **IOS** version to view the page.

## Prospective

We believe that EzTalk has a great potential in many aspects.

### User Perspective

EzTalk provides personalized recommendation for each users.

![User](/assets/user.png)

### Content Provider Prespective

EzTalk can also provide feedback for content providers.

![Provider](/assets/provider.png)

## Algorithm

![Algorithm](/assets/algorithm.png)