# mongo-express-k8s
Simple exercise to learn the basics of K8s service by creating a mongo express application


## Components
- Internal service for MongoDB (no external requests)
- "Mongo Express" deployment on the same network to ensure it can communicate with the MongoDB deployment
    - Mongo express is a web based interface for MongoDB. This will allow for us to interact with the MongoDB deployment from the browser/outside the network
- ConfigMap that contains the database URL
- Secret that contains the username and password
- Both of the above two will be referenced in the deployment files