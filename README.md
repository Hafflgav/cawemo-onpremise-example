# Cawemo OnPremise 
This repository should give an example how you can run Cawemo locally on your machine. Keep in mind that this is only 
possible when having access to the Enterprise Edition of Camunda. Make sure you have logged-in to the camunda regsitry before trying this out. 

## Documentation 
For more information you can always check out: https://docs.camunda.org/cawemo/latest/technical-guide/installation/.
Following this guide should give you a good starting point to understand and use this example. 

Besides of the steps in the documentation the following was done here: 
- Added two postgres container to the docker-compose. One for the data storage and one for the identity services. You could also use one container with two database inside. 
- Added a SMTP stub to the docker-compose.
- Use your devices IP address whenever needed. 
- Reference Garufa in the websocket section. 
- Check out the ports I have added inside of the env file. 

Make sure that you set all TLS or HTTPS related flags to false when running it locally. For generating the UUIDs you can use whatever tool you prefer. 
The instructions on how to generate a JWK can be found on the documentation linked above. 
