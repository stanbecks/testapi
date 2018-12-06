# testapi

Prerequisites:

    Install Node
    Install Newman
    npm install -g newman


	1. Get fixed token from todoist web > settings > integrations
	2. Replace the token value with the copied value in Test-project.postman_collection.json.
	3. Execute the command:
	   newman run "Test-project.postman_collection.json" --reporters cli,html --reporter-html-export ../nodeApp/report2.html
	   

Note:
Endpoints used:
https://beta.todoist.com/API/v8/projects
https://beta.todoist.com/API/v8/tasks

https://beta.todoist.com/API/v8/tasks endpoint has issues where failed when project_id is provided.