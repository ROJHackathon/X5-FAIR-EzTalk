# X5-FAIR-EzTalk
This file explains the problem statement, proposed solution and all the other details required to familiarise with the project idea.

## Contributors
This Project is made by Yangtao Ge([YangtaoGe518](https://github.com/YangtaoGe518)), ChoiLiam Wong([WongChoiLam](https://github.com/WongChoiLam)) and ([Zekun-Yang](https://github.com/Zekun-Yang))

Here is the detail responsibilities:
* *Yangtao Ge* is the team leader and the coordinator of the project; He also take responsibilities for front-end developing and project deployment.
* *ChoiLiam Wong* is the back-end developer who takes charge of server side for processing the API with Data; He also maintains the project document as well as API document.
* *ZeKun Yang* is the front-end developer who responses for implementing individual components.

## Problem Statement
Nowadays, there are seveal refugees from all over the world come to Europe for seeking asylum. However, they do not know the language used in the countries they are travelling to.
Also, culture confilt becomes a significant issue when those refugees are trying to intergrate into the new society. According to UN, this kind of language and culture problems becomes the sources
of violence, we should try to mitigate this problem.

Hence, the topic we choose is **Refugee Integration and Digital Education, Literacy & Refugee Children**.  There are two problems we are trying to solve
* **Lacking of personlized OERs(Online-Education Resources)** for refugees. Although, it exists several ways to obtain the resource, they are not easy to use and not for certain purposes(Culture and Langauge learning) which make it hard to use.
* **Lacking of platform to social with other people** who are under the same circumistances. Although, Facebook or WhatsApp provide a platform to communicate, they cannot provide a way of finding people who are also refugees exactly. Hence, a new platform of social integration should be developed specially for refugees.

## Proposed Solution
In order to solve the problem we stated above, we decide to develop a website pwa app called **EzTalk**, which is an app for language learning and language praticing.

This app has these following key features:
* Feed personlized OER according to the user preference
    * Language Learning Materials: Flashcard, learning videos & text, etc.
    * Culture background Materials: Travel guidence, Movie, Common Urban material etc.
* Customized Translation according to situation
* Chatroom for find people sharing the same hobby.

In addition, we decide for developing PWA(Progressive Web App) which is basically mobile-app-like website. It allows user can access the app by **only a url link** without downloading any apps.
This achieve our target of using convenience.

We also **X5GON's API** is used to retrive personlized data to produce a suitable and personlized feed. For example, it requires user to input their preference, records users search history, and also allows user to rate for the material they are feeded with.

## Project Structure
This project is collaborated on github orgnization([ROJHackathon](https://github.com/ROJHackathon)), all repositories are avaliable by this orgnization link.

The structure of the project is as following:
* [Back-End-EzTalk](https://github.com/ROJHackathon/Back-end-EzTalk):
     This server is developd on **Java Spring Boot**, which provides the API for front-end app to use. The backend server is deployed on a *private server* on *http://108.61.221.218:39802*. 
* [Front-End-EzTalk](https://github.com/ROJHackathon/Front-end-EzTalk):
    The user interface is developed on **React.js & Framework7**, which display the PWA in a *IOS* style layout.
* [Documents](https://github.com/ROJHackathon/Documents):
    Documents folder includes the general plan of developing.
* [API-Document](https://github.com/ROJHackathon/API-Documents):
    It is possinle API avaliable from the backend; Noticed that X5GON's APIs are encapuslated from the backend server, which can automatically analysis in backend.

## How to Deploy 
Since we have two parts -- Front-end and Back-end, we will discuss they individually:
### Back-end:
Here are two ways to run the server:
* **Directly access the website** (Recommanded): You can refer to the [API-Document](https://github.com/ROJHackathon/API-Documents) to trying getting any avaliable APIs on *[http://108.61.221.218:39802](http://108.61.221.218:39802)* 
* **Deploy on your own**: on local machine run `mvn clean package` to deploy the server. Then run `mvn spring-boot:run` to run the server `localhost:8080`

Although it is possible to run on your local machine, we *do not* recommanded to do so.

### Front-end:
Unlike server, you can run the clinet app on your local machine and it is recommanded. 

To build the project: `npm i` and run `npm start` to run the server. 

Since it is a PWA, we recommand to use *mobile mode* to view the project to get a better perspective, to do so:
* You may use **Google Chrome** to access developer tool.
* Change to any **IOS** version to view the page.
