# Jira Software : Docker-Project
# Video
https://github.com/user-attachments/assets/969c3817-dfda-40a5-868d-6874f80392f9
# Introduction
Jira Software is a project management tool tailored for agile teams. It facilitates the planning, tracking, and releasing of software projects at various scales, from small teams to enterprise-level operations. The tool supports popular agile methodologies like Scrum and Kanban, offering features such as sprint planning, backlog grooming, and real-time reporting for enhanced collaboration and productivity.
# Key Benefits
1. Ease of Deployment: Docker eliminates the need to manually configure the Jira environment. A simple command can start a fully operational instance.
2. Scalability: Docker containers can be scaled horizontally, making it easier to support larger teams or workloads.
3. Portability: The containerized nature ensures Jira runs consistently across various platforms, whether on-premises or in the cloud.
4. Efficiency: Running Jira in a Docker container reduces overhead by sharing resources efficiently with other containers on the same host.
# Steps Followed
The below command was used:-
1. Create a Docker Volume
   
`docker volume create --name jiraVolume`

2. Run the Jira Software Container
   
`docker run -v jiraVolume:/var/atlassian/application-data/jira --name="jira" -d -p 8080:8080 atlassian/jira-software`

3. Access Jira Software
   
`Jira is now available on http://localhost:8080`

