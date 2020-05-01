# SE35 - Software Modeling and Design Patterns

## 1. Diagrams

Diagrams can help to document and visualize the structure of a software project. One standardized way to describe specific parts of a software project is the Unified Modeling Language (UML) which is a standardized framework to visualize the structure/design of a software project. Additionally, you can also use other diagrams like ERD's or custom diagrams. In the next sections, I will describe some diagrams I have used during my project/in the past.

### 1.1 UML Sequence Diagram

The UML sequence diagram describes the communication between different parts of a system/different systems in time sequence. Furthermore, it helps to get an overview of which parts are communicating with each other in which order.

#### 1.1.1 OAuth2 flow
The following diagram explains the OAuth2 authentication flow in my application which is used to authenticate the user and receive access tokens to access protected resources:
![UML_Sequence_Auth_Flow.png](diagrams/UML_Sequence_Auth_Flow.png "")
<br/>

#### 1.1.2 MQTT authentication flow
The following diagram explains the authentication flow which is executed whenever a new client wants to connect to the MQTT broker:
![UML_Sequence_MQTT_Auth.png](diagrams/UML_Sequence_MQTT_Auth.png "")
<br/>

#### 1.1.3 Initialize device flow
This diagram describes the flow which is done during the production of an IoT device from the factory to initialize a new device in the system:
![UML_Sequence_Device_Factory.png](diagrams/UML_Sequence_Device_Factory.png "")
<br/>

#### 1.1.4 Device-claim flow
The following diagram describes the process of claiming an IoT device for a specific user who bought the device and wants to set it up:
![UML_Sequence_Claim_Device.png](diagrams/UML_Sequence_Claim_Device.png "")
<br/>

### 1.2 UML State Diagram
UML state diagram describes all possible states in which a software component can be in/transitioned to. This helps to get an overview of which events can happen to a component and what these events will change.

#### 1.2.1 App login states
The following diagram visualizes the states and event that can occur during the user login in the iOS app:
![UML_State_App_Login.png](diagrams/UML_State_App_Login.png "")
<br/>

#### 1.2.2 IoT device states
This diagram visualizes the possible states and state transitions of the IoT device:
![UML_State_IoT_Device_State.png](diagrams/UML_State_IoT_Device_State.png "")
<br/>

### 1.3 UML Package Diagram
The following package diagram shows a template of how I tried to structure all my REST API microservices which are implemented in Kotlin. This diagram describes the package structure so that all microservices share the same package structure and it is easy for other developers to work on different microservices without spending time on getting familiar with the project structure:
![UML_Package_Backend_Service_Template.png](diagrams/UML_Package_Backend_Service_Template.png "")
<br/>

### 1.4 UML Class Diagram
TODO 
<br/>

### 1.5 Custom diagrams
Despite the standardized UML diagrams I also used some custom diagrams to visualize some architectural concepts of my project. 

#### 1.5.1 General project architecture
The following diagram visualizes the overall architecture and all components of my project:
![Other_Architecture.png](diagrams/Other_Architecture.png "")
<br/>

#### 1.5.2 Cluster inbound network traffic
This diagram visualizes the network traffic routes into the Kubernetes cluster:
![Other_Networking_Inbound.png](diagrams/Other_Networking_Inbound.png "")
<br/>

### 1.6 Entity-Relationship-Diagram (ERD)
The Entity-Relationship-Diagram helps to visualize entities and their relationships with each other. This diagram is often used to visualize the database design for relational databases.

The services in my current project were very small and only had 2-3 entities so the ERDs were not necessary but I had a bigger database in a previous project. This is a screenshot of DataGrip and it is hard to see everything in this picture but if you use DataGrip to visualize the ERD it is possible to scroll and zoom in and out:
<br/>
![ERD_Keeet.png](diagrams/ERD_Keeet.png "")
<br/>

## 2. Design Patterns
