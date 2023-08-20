# azure-resume
My azure resume, following ACG project video

## First steps
- Frontend folder contains the website.
- main.js contains visitor counter code.

## Second steps
- Setting up Cosmos DB resources:
![Cosmos DB Item](frontend/AzR_Counter_item.png)
- Create Azure Function to interact with Cosmos DB counter data:
```js
const functionApi = 'http://localhost:7071/api/GetResumeCounter';
```
- Test Function locally to view counter data in browser:
 ![Website live counter](frontend/counter_liver.png)

## Third steps
- Deploy Azure Function to Azure, grab it's URL and update JavaScript code with it.
- Deploy static website to blob container.
- Setup Azure CDN for HTTPS and custom domain.

## Fourth steps
- Create frontend workflow. Create the GitHub workflow for deploying the frontend.
- Implement unit testing. Testing Azure Functions code in the deployment workflow.
- Create backend workflow. Create the GitHub workflow for deploying the backend.
![CI/CD Pipeline diagram](frontend/CICD_pipeline.png)