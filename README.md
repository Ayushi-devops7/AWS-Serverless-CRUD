## Serverless CRUD Application on AWS 

## 🚀 Project Overview  
This project demonstrates the creation of a fully functional **CRUD application** using AWS's serverless services. The application leverages **API Gateway**, **AWS Lambda**, and **DynamoDB** to showcase the potential of serverless architecture for building scalable and cost-effective solutions.  

---

## Key Highlights  

- **RESTful API Implementation**: Utilized **API Gateway** to handle HTTP requests seamlessly, ensuring smooth client-server communication.  
- **Serverless Processing**: Incorporated **AWS Lambda** to execute backend logic in response to triggers from API Gateway.  
- **Data Management**: Designed an efficient and scalable database solution using **DynamoDB** for storing and retrieving data.  
- **Scalability**: The serverless architecture adapts dynamically to varying loads, eliminating the need for manual scaling.  

---

## Architecture  
The application is built around the following core components:  

1. **API Gateway**: Acts as the entry point for HTTP requests and routes them to the appropriate Lambda functions.  
2. **AWS Lambda**: Processes business logic for each CRUD operation (Create, Read, Update, Delete).  
3. **DynamoDB**: Stores application data in a NoSQL database optimized for serverless applications.  

---

## Features  

- **Create**: Add new records to the DynamoDB database.  
- **Read**: Retrieve existing records via API requests.  
- **Update**: Modify specific fields of existing records.  
- **Delete**: Remove records from the database.  

---

## Technologies Used  

- **Amazon API Gateway**  
- **AWS Lambda**  
- **Amazon DynamoDB**  
- **AWS CloudFormation** (Optional for deployment)  

---

## How to Create This Project  

### **Setup Your AWS Environment**  
1. **Create an AWS Account** if you don’t already have one.  
2. Use the AWS Management Console to access services.  

---

### 2️⃣ **Create the DynamoDB Table**  
1. Navigate to the **DynamoDB** service in the AWS Management Console.  
2. Click **Create Table**.  
3. Provide the following details:  
   - **Table Name**: `CRUDTable`  
   - **Partition Key**: `id` (Type: String)  
4. Leave other settings as default and click **Create Table**.  

---

### 3️⃣ **Develop Lambda Functions**  
1. Write Lambda functions for each CRUD operation:  
   - **Create Item**: Insert data into DynamoDB.  
   - **Read Item**: Fetch data based on the `id`.  
   - **Update Item**: Modify existing data.  
   - **Delete Item**: Remove data based on the `id`.
   -  
---

### 4️⃣ Set Up API Gateway
1. Navigate to API Gateway in the AWS Management Console.
   - **Create a REST API** and define resources for each CRUD operation:
   - /create → POST → Link to Create Lambda
   - /read/{id} → GET → Link to Read Lambda
   - /update → PUT → Link to Update Lambda
   - /delete/{id} → DELETE → Link to Delete Lambda
2. Enable CORS for the API Gateway methods.
   
---

### 5️⃣ Test the Endpoints
 - Deploy the API to a Stage (prod).
 - Use tools like Postman to send HTTP requests to the API endpoints.
 - Validate data in the DynamoDB table using the AWS Management Console.

---

### 6️⃣ Monitor and Optimize
- Enable CloudWatch Logs for each Lambda function to monitor execution.
- Optimize Lambda functions by reducing memory usage and execution time.
- Implement retries and error handling for better reliability.

---

### Best Practices
  - Use IAM roles and policies to securely access AWS resources.
  - Enable CloudWatch logging to monitor application performance.
  - Optimize Lambda functions for performance and cost efficiency.
  - Implement input validation to ensure data integrity.

---

### Outcome
This project highlights the efficiency of serverless architectures for modern application development. It’s a step forward in building reliable, scalable, and cost-efficient solutions on the cloud.

### Contact
If you have any questions or would like to discuss this project further, feel free to connect with me on https://www.linkedin.com/in/ayushi-agrawal-2636b9266 or email me at ayushiagrawal571@gmail.com.

Happy Coding! 😊
