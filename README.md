# Dynamic-real-time-large-screen-bank-supervision-system-based-on-Echarts-SpringBoot
## 1.Project Description
The project is to create a dynamic real-time large screen supervision system for banks. The project is based on LED screen with 16:9 aspect ratio. Echarts + SpringBoot framework is used for development.

## 2.Effect demonstration
A variety of data information can be displayed dynamically and in real time. Right mouse button to change the theme style.

![bank system 01](https://user-images.githubusercontent.com/89632568/221911989-d9b17243-9de6-44a1-8e20-a5e19df7e53e.png)
![bank system 02](https://user-images.githubusercontent.com/89632568/221912051-14f310d3-c30b-4a29-bedb-dccdcf561a5f.png)

## 3.Project deployment
Based on free installable executable program: supports Windows, Linux, Mac and other operating systems; the program can be copied to the server without any other environmental dependencies; users can either view the program interface directly on the server or open and play it with a browser from a remote location.

## 4.Overall architecture design
a. Front-end design based on the Echarts open source library, using the WebStorm editor.\n
b. Back-end based on Java Web implementation, using the IDEA editor.\n
c. Data transfer format: JSON.\n
d. Data source type: currently using JSON file method , add Mybatis can support PostgreSQL, MySQL, Oracle, Microsoft SQL Server, SQLite , add POI can support Excel tables , etc. , you can also customize the HTTP API interface method .\n
e. Data update method: use http get polling method . In practice, you can also choose to monitor the back-end data update in real time, depending on the situation, real-time push to the front-end way.

## 5.Development configuration & Code structure
### a.SpringBoot configuration
Spring Boot is a new JAVA open source application framework provided by the Pivotal team and is designed to simplify the initial build and development process of new Spring applications. Configuring SpringBoot is a very simple task. Start by typing "Spring.io" into your browser to get to the Spring homepage. Click on QUICKSTART to enter the SpringBoot project configuration screen. The project is based on Maven development, using JAVA language, SpringBoot version is 2.7.9, packaging type is jar package, Java language version is 8.

![bank system 04](https://user-images.githubusercontent.com/89632568/221913890-8d22c95d-8aa7-4cbb-ba63-b064009e0523.png)

### b.Json configuration
JSON is a lightweight data interchange format . It is based on ECMAScript and uses a text format to store and represent data completely independent of the programming language. The simplicity and clarity of the hierarchy make JSON the ideal language for data interchange. Easy to read and write by humans, but also easy to parse and generate by machines, it can effectively improve the efficiency of network transmission. The project uses alibaba's json library, and the pom.xml file adds the following configuration.

![image](https://user-images.githubusercontent.com/89632568/221914134-045f33b6-3155-4928-bf20-fa9441b33d44.png)

### c. Code structure
#### (I). Static path
Static files are located under the Static directory. Mainly store images, display formats and other related resource files.
![bank system 代码架构](https://user-images.githubusercontent.com/89632568/221915162-2185a7c5-2243-4d56-a46f-2f51c536b7b5.png)

#### (II). Java directory
Process is the main Java code, used to handle Json communication data.
![bank system java](https://user-images.githubusercontent.com/89632568/221915221-532183c7-420e-40e7-a503-f78fe63c5cfa.png)

#### (III). Port configuration
Application.properties file configures the web service listening port. Usually the default is 80.
![bank system 端口](https://user-images.githubusercontent.com/89632568/221915280-99228748-0c44-43c9-bb8b-bae63090f780.png)

#### (IV). Start and run
Start the project in the compiler, you can see the console printout Spring framework. The listening port number is 80. Enter the URL in the browser to see the results [http://localhost:80].
![bank system 启动](https://user-images.githubusercontent.com/89632568/221915345-e948d6be-f401-4625-9d47-961f4fc2a4be.png)
![bank system 03](https://user-images.githubusercontent.com/89632568/221915437-726f57f1-b94e-4a01-803c-0d927dbb361f.png)


