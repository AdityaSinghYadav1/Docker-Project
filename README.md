# Jira Software : Docker-Project
# Introduction
Jira Software helps the agile teams plan, track, and release great software at scale. This Docker container makes it easy to get an instance of Jira Software.
# Steps Followed
The below command was used:-
docker volume create --name jiraVolume
docker run -v jiraVolume:/var/atlassian/application-data/jira --name="jira" -d -p 8080:8080 atlassian/jira-software
Jira is now available on http://localhost:8080

