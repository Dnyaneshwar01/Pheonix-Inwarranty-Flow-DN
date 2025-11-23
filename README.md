About the project: 
This repository contains a Postman API Test Collection designed to run using Postman UI, Newman CLI, Jenkins, and GitHub Actions. It provides a simple, maintainable, and CI-ready solution for automated API testing without needing a full programming framework.

With Newman, the collection can be executed locally or integrated into CI/CD pipelines, making it suitable for smoke tests, regression suites, and continuous validation across environments.

How to run the Project?

You can run the project on your local system for that:

Clone the Project on Local System: https://github.com/Dnyaneshwar01/Phoenix-Inwarranty-Flow.git

Install Nodejs and NPM from https://nodejs.org/en

Install Newman using npm install -g newman

Install Newman-reporter-htmlextra npm install -g newman-reporter-htmlextra

Run the Newman Command:

       newman run 'Inwarranty-flow Collection.postman_collection.json' \  
      -e QA.postman_environment.json \
      -d testdata.csv \
      -r cli,htmlextra \
      --reporter-htmlextra-export ./newman/index.html 
