This repository contains a set of automated API tests written using Postman and can be executed via the CLI (Newman) or directly within the Postman app. 

 

Prerequisites 

Ensure the following tools are installed on your system: 

Tool 

Recommended Version 

Node.js 

v18 or above 

Postman 

Latest 

 

Getting Started 

1. Create and Navigate to a Project Folder 

Create a folder where you want to install this project. Then open your terminal and navigate into it. 

mkdir my-postman-project 
cd my-postman-project 
 

 

2. Clone the Repository 

Clone this GitHub repository into the folder and navigate into the cloned directory: 

git clone https://github.com/Darmolyna/BuildasPostman.git 
cd BuildasPostman 
 

 

3. Run API Tests from the CLI (Newman) 

Use the following command to run the tests and generate an HTML report: 

npx newman run "path/to/your/postman_collection.json" \ 
  --reporters cli,html \ 
  --reporter-html-export newman-reports/report.html 
 

⚠️ Note: 
 Replace path/to/your/postman_collection.json with the actual path to your Postman collection file 

Example for macOS: 

npx newman run "/Users/Blessing/Downloads/Blessing Olaiya Buildas Postman.postman_collection.json" \ 
  --reporters cli,html \ 
  --reporter-html-export /Users/Blessing/Downloads/newman-reports/reports.html 
 

 

4. Run Tests in Postman UI 

You can also run the tests directly within Postman: 

Open the Postman app. 

Click Import (top left). 

Choose the BuildasPostman.postman_collection.json file you cloned from GitHub. 

Once imported, go to the Collections tab. 

Click the collection name → right click on it and select Run. 

Configure run settings (e.g., iteration count, environment, etc.) and click Run. 

 # Postman GitHub Actions
