# Coding Challenge

## Requirements:

1.	Write an API endpoint that accepts a GitHub ID and returns Follower GitHub ID’s (up to 5 Followers total) associated with the passed in GitHub ID.  Retrieve data up to 3 levels deep, repeating the process of retrieving Followers (up to 5 Followers total) for each Follower found.  Data should be returned in JSON format.
2.	Code should be checked into a public GitHub repository, so that the CenturyLink team members can review your code at any time.
3.	A readme file should be included and checked into GitHub with instructions on how to execute and test your API.
4.	Bonus credit: API endpoint is publicly accessible and fully functional, so that CenturyLink team members can execute and test your API at any time.

## Bonus Challenge:

The bonus challenge NOT required!

1.	Write an API endpoint that accepts a GitHub ID and retrieves the Repository names (up to 3 Repositories total) associated with the passed in GitHub ID, along with the Stargazer GitHub ID’s (up to 3 Stargazers total) associated with each Repository.  Retrieve data up to 3 levels deep, repeating the process of retrieving the associated Repositories (up to 3 Repositories total) for each Stargazer (up to 3 Stargazers total) found.  Data should be returned in JSON format.
2.	See requirements 2, 3, and 4 above.

## Tips:

1.	You’ll need a GitHub account (which are free) to complete this coding challenge.
2.	GitHub provides API’s for retrieving Followers, Repositories, and Stargazers.  Please see the following GitHub API documentation:

	a.	https://developer.github.com/v3/users/followers/

	b.	https://developer.github.com/v3/repos/

	c.	https://developer.github.com/v3/activity/starring/


# Pre-reqs
To build and run this app locally you will need a few things:
- Install [Node.js](https://nodejs.org/en/)
- Install [MongoDB](https://docs.mongodb.com/manual/installation/)
- Install [VS Code](https://code.visualstudio.com/) (you can use any)


# Getting started
- Clone the repository
```
git clone <name of repositry>
```
- Install dependencies
```
cd <project_name>
npm install
```
- Configure your mongoDB server
```bash
# create the db directory
sudo mkdir -p /data/db
# give the db correct read/write permissions
sudo chmod 777 /data/db
```
- Start your mongoDB server (you'll probably want another command prompt)
```
mongod
```
- Run the project
```
npm start
```

### Github Followers

To receive the first 5 followers of a github user, 3 levels deep, append either the local url with:

/:username/followers

Where "username" is the github username.

### Github Repos

To receive the first 3 repositories of a github user, and the first 3 stargazers of the repo, append either the local url with:

/:username/repos

Where "username" is the github username.