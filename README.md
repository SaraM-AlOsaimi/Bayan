
<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="">
<img src="images/tuwaiq.png" alt="logo" width="152" height="100">
<img src="images/bayan.png" alt="logo" width="152" height="100">
 
</a>
 
<h3 align="center">Bayan</h3>

  <p align="center">
  This final project wraps up the Java Spring Boot Web Application Development bootcamp at Tuwaiq Academy.
 <br />
    <a href="https://www.figma.com/design/zTIO7kQz6k6514lARuOtXo/Untitled1?node-id=0-1&p=f&t=1OL4NiM8cWGly5It-0">Figma</a>
    ·
    <a href="https://documenter.getpostman.com/view/40740226/2sAYJAcwpL">Postman API</a>
    ·
    <a href="https://github.com/salemALmotiry/Bayan/issues">Request Feature</a>
  </p>



<!-- ABOUT THE PROJECT -->
## About The Project
Bayan is a specialized platform designed to streamline customs clearance processes by connecting clients, 
whether individuals or companies, with certified customs brokers. 
Bayan offers an advanced shipment management system,
supported by innovative tools that help reduce time and effort while simplifying customs procedures.

بيان هي منصة متخصصة تهدف إلى تسهيل عمليات التخليص الجمركي من خلال ربط العملاء، سواء كانوا أفرادًا أو شركات، بمخلصين جمركيين معتمدين. تقدم بيان نظامًا متطورًا لإدارة الشحنات، مدعومًا بأدوات مبتكرة تُسهم في تقليل الوقت والجهد وتبسيط الإجراءات الجمركية.



<!-- ABOUT THE PROJECT -->
## 🛠 Key Features

### **Customer and Broker Reviews**
Facilitate mutual feedback with ratings and reviews to enhance collaboration.

---

### **Order Management**
Simplify order processing, track shipments, and manage delivery statuses effortlessly.

---

### **Shipment Tracking**
Track shipments with precision using various supported providers:

#### Small and Medium Shipments (Air and Land Logistics):
- **Aramex**
- **Naqel**
- **DHL**

#### Large Shipments (Air and Sea Logistics):
- **Saudi Cargo** (Air – specializes in large shipments)
- **MSC** (Sea – handles large cargo)

---

### **Offer and Request Handling**
Seamlessly create requests, receive offers, and manage collaboration with customs brokers.

---

### **File Management System**
Upload, organize, and download shipment-related documents with ease.

---

### **Notifications and Alerts**
Stay informed with instant updates through email and SMS notifications.


## Diagram
![img.png](img.png)
<!-- LIVE VERSION -->

## User cases
![image](https://github.com/user-attachments/assets/44bb88da-2b41-4cf2-82bd-64e8a707ab90)
![image](https://github.com/user-attachments/assets/50c32047-16e0-4025-84fb-0b57b66e7916)
![image](https://github.com/user-attachments/assets/3ae585af-cfe2-4b43-a2aa-85fa439262da)
![image](https://github.com/user-attachments/assets/8eed383e-5e78-4a1d-9e8d-17e3fdf6f797)
<!-- Contributing -->

---
## Models
| **Model Name**   |
|------------------|
| CustomeBroker    |
| Address          |
| Delivery         |
| SubscriptionPost |

## CRUD Operations  
   - Address
   - Delivery
   - Post
## Extra endpoint

| **HTTP Method** | **Relative Path**                                    | **Service Method**                |
|----------------|------------------------------------------------------ |---------------------------------- |
| POST           | `/add`                                                | `addPost`                         |
| GET            | `/my-posts                      `                     | `getMyPosts`                      |
| GET            | `/get-all-posts`                                      | `/get-all-posts`                  |
| POST           | `/send-ad-to-broker/{brokerId}`                       |  `sendPostForOneBroker`           |
| GET            | `/broker/posts`                                       | `getPostsForBroker`               | 
| POST           | `/create-offer`                                       | `createOffer`                     |
| POST           | `/add-address`                                        | `addAddress`                      |
| GET            | `/my-addresses`                                       | `myAddress`                       |
| PUT            | `/accept-custom-broker/custom-broker/{customerId}`    | `acceptCustomBroker`              |
| PUT            | `/reject-custom-broker/custom-broker/{customerId}`    | `rejectCustomBroker`              |
| GET            | `/custom-brokers`                                     | `getAllCustomBrokers`             |
| GET            | `/custom-brokers/waiting-for-acceptance`              | `getBrokersWaitingForAcceptance`  |
| GET            | `/get-all-my-notifications`                           | `getAllNotifications`             |
| PUT            | `/read-my-notifications/{notificationId}/mark-as-read`| `markNotificationAsRead`          |
| POST           | `/register`                                           | `register`                        |
| DELETE         | `/remove-border/{borderId}`                           | `/remove-border/{borderId}`       |
| GET            | `/my-profile`                                         | `myProfile`                       |
| GET            | `/display-all-custom-brokers`                         | `getAllCustomsBrokers`            |
| GET            | `/license-number/{licenseNumber}`                     | `getByLicenseNumber`              |
| GET            | `/border/{border}`                                    | `getAllCustomsByBorder`           |
| GET            | `/name/{name}`                                        | `getAllCustomsByName`             |
| GET            | `/license-type/{type}`                                | `getAllCustomsByLicenseType`      |
| PUT            | `/accept-offer/{offerId} `                            | `acceptOffer`                     |
| GET            | `/all-offer-post/{postId},`                           | `getAllOffersForOnePost`          |

---

### DTO Files

| **Type**  | **Name**               |
|-----------|------------------------|
| IN        |AddPostDTO              |
| IN        |ReviewCustomerDTO       |
| IN        | UpdateCustomerDTO      |
| IN        |UpdateCustomsBrokerDTO  |
| OUT       | ReviewDTO              |
| OUT       |OrderDTO                |
| OUT       | OfferDTO               |
| OUT       | DocumentsDTO           |
| OUT       | DeliveryDTO            |
| OUT       | NotifationDTO          |
| OUT       | CustomerDTO            |
| OUT       | CustomerRentalsDTO     |
| OUT       | CustomerOfferDTO       |


## Testing Frameworks  
- **JUnit** –  Used for testing, Controller layer validation.  

### Built With
This project was built using:

- **Java SE**
- **IntelliJ IDEA**
- **MySQL**
- **Spring Boot**
- **AWS**
- **Ultramsg**
- **Spring Boot Mail Integration**
- **Postman**
- **Git**
- **DataGrip**
- **Selenium**
- **ChromeDriver**


<!-- License -->

## 📝 License

This project is [MIT](https://opensource.org/licenses/MIT) licensed.
