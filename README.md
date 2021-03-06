# API Test Automation framework
Boilerplate API test framework using Mocha, SuperTest and TypeScript.

#### Pre-requisite:
[![NodeJs](https://img.shields.io/badge/-NodeJS%20v10%20OR%20later-%23339933?logo=npm)](https://nodejs.org/en/download/)
[![VSCode](https://img.shields.io/badge/-Visual%20Studio%20Code-%233178C6?logo=visual-studio-code)](https://code.visualstudio.com/download)

#### Getting Started:
Clone Repository
```bash
1. git https://github.com/sadabnepal/APITestFrameworkMochaTS.git
2. Navigate to APITestFrameworkMochaTS
```

Install the dependencies
```bash
npm install
```
Run tests
```bash
npm test
```

Report Path:
```
path: <PROJECT_FOLDER>/report/mochawesome.html
```

GitHub Actions:
> With Each push on master branch all test will be executed using github action and docker image.
> Post execution report will be copied to github artifact which can be later downloaded.
```
Path: https://github.com/sadabnepal/APITestFrameworkMochaTS/actions
```

Docker Run:
> Setup [docker](https://docs.docker.com/get-docker/) in your local machine to run test in dockerize environment
```
docker build -t node-api-image . [ you can given any name of your choice ]
docker run node-api-image:latest [ to run test inside docker ]
```

#### Features:
    - Mocha Framework with Mochawesome report integration
    - Custom types for better code intellisense
    - Service as enum for better input control
    - Schema validation
    - Multi environment support  
    - JSON file as data source
    - Docker and Github integration
    - Enhanced import statements
    - Report response logger

#### Tech stacks:
[![SuperTest](https://img.shields.io/badge/-SuperTest-07BA82?logoColor=white)](https://github.com/visionmedia/supertest)
[![TypeScript](https://img.shields.io/badge/-TypeScript-%233178C6?logo=Typescript&logoColor=black)](https://www.typescriptlang.org/)
[![Mocha](https://img.shields.io/badge/-Mocha-%238D6748?logo=Mocha&logoColor=white)](https://mochajs.org/)
[![ChaiJS](https://img.shields.io/badge/-ChaiJS-FEDABD?logo=Chai&logoColor=black)](https://www.chaijs.com/)
[![Docker](https://img.shields.io/badge/-Docker-0db7ed?logo=docker&logoColor=white)](https://www.docker.com/)

#### Folder Structure:
```
????????????.github [ github action integration ]
????????????.vscode [ auto code and import formatter ]
????????????src
|     ????????????config [ basic configuration]
|     ????????????helper [ resuable components ]
|     ????????????resources [ data and schema files ]
|     ????????????services [ endpoint and header files ]
|     ????????????test
|     ????????????types
????????????.gitignore
????????????Dockerfile [ build docker image ]
????????????package-lock.json
????????????package.json
????????????README.md
????????????tsconfig.json
```

#### Sample Report
![SamplReport](https://user-images.githubusercontent.com/65847528/167574833-05db8fe3-e2b0-4d97-9cac-16f6f1c6c0c2.png)