# Remote Code Executor

Remote Code Executor (RCE) as the name suggests, is an online code executor like seen on Leetcode, etc. For the project, we have implemented an _**infinitely scalable**_ code executor to run a code snippet. It will create a new file for each code input, execute it and returns the output. It supports major languages, i.e., C/C++, Python, Javascipt, Java and can even be extended to support more languages.

## Screenshots
<img src="https://github.com/sohan2410/RCE-frontend/blob/main/public/static/images/flow2.png"></img>
<img src="https://github.com/sohan2410/RCE-frontend/blob/main/public/static/images/rce-dark.png"></img>
<img src="https://github.com/sohan2410/RCE-frontend/blob/main/public/static/images/rce-light.png"></img>

## Hosted URL
#### Frontend
- [Hosted Link](https://rce-nine.vercel.app)
- [Repo Link](https://github.com/DarikshaAnsari/RCE_Frontend)
#### Backend
- [Hosted Link](https://3m0vak6ytg.execute-api.ap-south-1.amazonaws.com/default/test)
- [Repo Link](https://github.com/DarikshaAnsari/RCE_Backend)
## Features Implemented

- Infinitely Scalable Code
- Code Sanitization
- Time limited execution
- Drag and Drop code and input
- Download code snippet
- Resize the font of the editor
- Light/Dark Mode
- Code Suggestion and Autocompletion

## Concepts used
- Application is made infinitely scalable by utilizing the concept of serverless architecture, which is implemented with the help of the Serverless Framework and AWS Lambda Functions. 
- ```exec``` from NodeJS Child process module was used to execute the code snippets in a shell.
- Docker was used to containerize the application which contains all the required dependencies and that image is utilized for AWS Lambda functions.
- A CI/CD pipeline was setup using Github Actions for quick deployment.
<img src="https://github.com/sohan2410/RCE-frontend/blob/main/public/static/images/flow.png"></img>
## Technologies/Libraries/Packages Used
| Packages |  |
| ------ | ------ |
|NextJS| To build frontend application  |
|Ace Editor|Online IDE Code Editor|
|AWS Lambda|Serverless Compute service|
|Cloudwatch|Monitor lambda function logs|
|API Gateway|To trigger lambda functions|
|Docker|To build containerized applications|
|Serverless framework|To build serverless applications|

## Local Setup

### Frontend
1. Clone frontend repository from [here](https://github.com/DarikshaAnsari/RCE_Frontend)
```shell
git clone https://github.com/DarikshaAnsari/RCE_Frontend.git
```
2.  Install all package dependencies (one time operation)
```shell
npm install
```
3. Run using command
```shell
npm run dev
```

### Backend
1. Clone backend repository from [here](https://github.com/sohan2410/RCE-backend)
```shell
git clone https://github.com/DarikshaAnsari/RCE_Backend.git
```
2.  Install all package dependencies (one time operation)
```shell
npm install
```
3. Run using command
```shell
npm run dev
```
