# Bayan System

**Bayan** is a specialized platform aimed at facilitating customs clearance processes by connecting clients, whether individuals or companies, with reliable customs brokers. **Bayan** provides an advanced shipment management system, supported by innovative tools designed to save time and effort, offering a secure and easy customs experience infused with trust.

---

## 🛠 Key Features

- **Connecting Customs Brokers**  
  Easily connect with accredited and reliable customs brokers to receive professional clearance services.

- **Advanced Shipment Management**  
  An integrated system for managing shipments, including tracking, document organization, and process optimization.

- **Real-Time Tracking**  
  Monitor shipment statuses instantly with full transparency.

- **Automated Documentation**  
  Tools for creating and managing customs documents automatically, reducing errors and saving time.


- **Analytics and Reporting**  
  Comprehensive tools for insights and reports on shipment operations to improve performance.

---

## 🌍 منصة بيان

**بيان** هي منصة متخصصة تهدف إلى تسهيل عمليات التخليص الجمركي من خلال ربط العملاء، سواء كانوا أفرادًا أو شركات، بالمخلصين الجمركيين الموثوقين. توفر **بيان** نظامًا متطورًا لإدارة الشحنات، مدعومًا بأدوات مبتكرة تُعنى بتوفير الوقت والجهد، لتقديم تجربة جمركية آمنة وسهلة يتخللها الثقة.

---

### ⭐️ الميزات الرئيسية

- **ربط المخلصين الجمركيين**  
  الاتصال بمخلصين جمركيين معتمدين وموثوقين للحصول على خدمات تخليص احترافية.

- **إدارة الشحنات المتقدمة**  
  نظام شامل لإدارة الشحنات يتضمن التتبع وتنظيم الوثائق وتحسين العمليات.

- **التتبع في الوقت الحقيقي**  
  متابعة حالة الشحنات بشفافية كاملة.

- **توثيق آلي**  
  أدوات آلية لتوثيق المستندات الجمركية، تقلل الأخطاء وتوفر الوقت.

- **معالجة مدفوعات آمنة**  
  نظام دفع آمن بخيارات متعددة لتلبية احتياجات العملاء.

- **دعم العملاء**  
  فريق دعم مخصص لتقديم المساعدة في الاستفسارات أو المشاكل.

- **تحليلات وتقارير**  
  أدوات شاملة للحصول على رؤى قيمة وتحسين الأداء.

---

## 🔗 Links and Resources

- [Figma Design](#)  
- [Presentation](#)  
- [Postman API](https://documenter.getpostman.com/view/40740226/2sAYJAcwpL)  
- [Diagrams Part 1](#)  
- [Diagrams Part 2](#)

---
## Diagram
![image](https://github.com/user-attachments/assets/f8633fc7-8efe-4132-9a1e-bdd2a552a960)

## User cases 
![image](https://github.com/user-attachments/assets/44bb88da-2b41-4cf2-82bd-64e8a707ab90)
![image](https://github.com/user-attachments/assets/50c32047-16e0-4025-84fb-0b57b66e7916)
![image](https://github.com/user-attachments/assets/3ae585af-cfe2-4b43-a2aa-85fa439262da)
![image](https://github.com/user-attachments/assets/8eed383e-5e78-4a1d-9e8d-17e3fdf6f797)

----
## 👩‍💻 My Work on the Project

As part of developing the **Bayan** platform, I implemented the following:

### 🚀 Features Developed

1. **Model**  
   - Customer
   - CustomBroker
   - Delivery
   - MyUser
2. **CRUD Operations**  
   - Address
   - Delivery
   - Post


3. **Extra Functionalities**  
## قائمة النقاط النهائية (API Endpoints)

| **طريقة HTTP** | **المسار النسبي**                                    | **ميثود الخدمة**                |
|----------------|------------------------------------------------------|----------------------------------|
| POST           | `/add`                                               | `addPost`             |
| GET            | `/my-posts                      `                    | `getMyPosts`           |
| GET            | `/get-all-posts`                                     | `/get-all-posts`             |
| POST            | `/send-ad-to-broker/{brokerId}`                      | `sendPostForOneBroker`           |
| GET            | `/broker/posts`                                       | `getPostsForBroker`       |
| POST            | `/create-offer`                                       | `createOffer`                    |
| POST            | `/add-address`                                        | `addAddress`                   |
| GET            | `/my-addresses`                                       | `myAddress`                     |
| PUT            | `/accept-custom-broker/custom-broker/{customerId}`    | `acceptCustomBroker`               |
| PUT            | `/reject-custom-broker/custom-broker/{customerId}`    | `rejectCustomBroker`              |
| GET           | `/custom-brokers`                                     | `getAllCustomBrokers`              |
| GET           | `/custom-brokers/waiting-for-acceptance`               | `getBrokersWaitingForAcceptance`  |
| GET            | `/get-all-my-notifications`                             | `getAllNotifications`            |
| PUT            | `/read-my-notifications/{notificationId}/mark-as-read` | `markNotificationAsRead`         |
| POST           | `/register`                                           | `register`                      |
| DELETE         | `/remove-border/{borderId}`                           | `/remove-border/{borderId}`   |
| GET            | `/my-profile`                                          | `myProfile`                       |
| GET            | `/display-all-custom-brokers`                         | `getAllCustomsBrokers`           |
| GET            | `/license-number/{licenseNumber}`                     | `getByLicenseNumber`          |
| GET            | `/border/{border}`                                    | `getAllCustomsByBorder`          |
| GET            | `/name/{name}`                                       | `getAllCustomsByName`            |
| GET            | `/license-type/{type}`                                 | `getAllCustomsByLicenseType`    |
| PUT            | `/accept-offer/{offerId} `                          | `acceptOffer`                     |
| GET            | `/all-offer-post/{postId},`                          | `getAllOffersForOnePost`          |

## القسم الأول

| **المجلد**    | **الاسم**       |
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
| OUT       | CustomerRentalsDTO      |
| OUT       | CustomerOfferDTO        |

4. **API Development**  
   Designed and implemented APIs for shipment tracking and management.
5. **J Usent Test**
   -Test Get All Posts
   -Test Add Post
   -Test Delete Post
   -Test Update Post
   -Test Get My Posts

---

## 📂 Tags

- **#CustomsClearance**  
- **#ShipmentManagement**  
- **#RealTimeTracking**  
- **#SecurePayments**  
- **#CustomerSupport**  
- **#Analytics**  
- **#API**  
- **#Testing**
