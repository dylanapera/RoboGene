# Azure Spend Support Chatbot | [RoboGene](https://robogene.azurewebsites.net/)

## **Overview**
This chatbot is designed to assist **business users** in managing and understanding their **Azure spend**. It provides detailed breakdowns by:
- **Service Type**
- **Service Cost**  
The solution focuses exclusively on **Azure services**.

---

## **Key Features**
- **Query Azure Spend Data**  
  - Users can query **SQL Database** for cost and service details.
- **AI Integration**  
  - Built using **Agent Builder** in **AI Foundry**.
- **Web Hosting**  
  - Hosted on **Azure Web App** for scalability and security.

---

## **Architecture**
### **Components**
1. **Azure SQL Database**
   - Stores service type and cost data.
2. **AI Foundry Agent Builder**
   - Powers the chatbot logic and natural language understanding.
3. **Azure Web App**
   - Hosts the chatbot interface for end-users.

---

## **Workflow**
1. **User Interaction**
   - Business user queries cost breakdown.
2. **Chatbot Processing**
   - AI Agent interprets query.
3. **Database Query**
   - Fetches service type and cost from Azure SQL DB.
4. **Response**
   - Displays structured cost details in the chatbot UI.

---

## **Tech Stack**
- **Azure SQL Database**
- **Azure Web App**
- **AI Foundry Agent Builder**
- **Azure SDK for integration**

---
## Contibutors
Scott and Dylan
## **Example Query**
```sql
SELECT ServiceType, ServiceCost
FROM AzureSpend
WHERE ServiceType = 'Virtual Machines';
