# kondoboard-cron

This repo contains the extract, transform, load application for Kondoboard, a platform that allows Lambda School students to browse, save, and track job postings during the job hunt. 

## Table of Contents
- [Diagrams](#diagrams)
- [Install](#install) 
- [Usage](#usage)
- [Testing](#testing)
- [API](#api)
- Future Features
- [License](#license)


## Diagrams
We created C4 diagrams to communicate the software architecture

### Context
![Context](./diagrams/kondo_context.svg)
### Container
![Container](./diagrams/kondo_container.svg)

## Install  
```
pip install -r requirements.txt
```
## Usage  
```
uvicorn main:app --reload
```  
## Testing  
```
pytest
```  
## API

[FastAPI - Swagger documentation](http://kondoboard-ds-environment.eba-u7c3zdzn.us-east-1.elasticbeanstalk.com/docs)  

## Future Features

- Find a better solution for hosting the ETL - resources are being wasted having all of that code hosted 24/7 if we only need access to it 2x / day. This will require the use of Docker
- Add the ability to search for remote only positions. We will need to label jobs we are already pulling in as well as source some jobs from APIs like Remotive
- Handle missing location tags better
 
## License
![License](./LICENSE/)
