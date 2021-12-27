# Akvelon-TaskTracker-AllFiles
Test task for internship
Project include two controllers that allows you to work with Project and Task entities.
Data Transfer Object, Repository pattern were used in the project.

Project entity has the following data:
      Id (int)
      Name (string)
      Description (string)
      Priority (int)
      Status (enum: NotStarted, Active, Completed)
      Start time
      Completion time
      Set of Tasks
      
Task entity has the following data:
      Id (int)
      Name (string)
      Description (string)
      Status (enum: ToDo, InProgress, Done)

Filtering and sorting of Projects is implemented in the project.
All API documentations is provided in Swagger.

Here is requests hierarchy:
Projects:	
api/projects	
	GET
	POST
	PUT
api/projects/{project_id}
	GET
	DELETE
  PATCH

Tasks:
api/projects/{project_id}/tasks
	GET
	POST

api/projects/{project_id}/tasks/{id}
	GET
	DELETE
