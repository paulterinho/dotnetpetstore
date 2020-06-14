# Swagger Petstore Auto Gen Tests for C#

Just a simple example to shamelessly try to influence my wonderful colleagues (see what I'm doing there? hahahah. ) in an effort to adopt this very useful technology. 

This Techonology will allow us to 
  1) Understand any given API at a glance (it will have an updated list of all API methods), 
    - Even allow us to specify what exceptions we should expect.
  2) Allow us to Mock a service we don't have access to.
  3) Auto-generate tests based on our Swagger/OpenAPI contract.
  4) Speed development time (you can create a stubbed service for which ever piece you aren't working on)
    - an example of this is if you working on a server piece, you can create a hook to automatically resend a request everytime you save, thus saving you the need to go to Postman, line up the three requests to set up the one you are interested in, and then remove that request's consequences so you can retest it. 

## Running code
- Use "Visual Studio Code" IDE and not "Visual Studio". (See notes in the Appendix for more info)

## Viewing Swagger / Open API Documents:
- Swagger Editor: `http://localhost:5000/swagger/index.html`
- Swagger JSON: `http://localhost:5000/swagger/1.0.0/swagger.json`

## Auto Generate the Swagger / OpenAPI document 
- This is the library that generates Swagger/OpenAPI documents from existing code bases
- `https://github.com/domaindrivendev/Swashbuckle.AspNetCore`

## Auto Generate the Server and Client Stubs.
- https://github.com/swagger-api/swagger-codegen/issues/2276
- https://github.com/swagger-api/swagger-codegen

## Appendix
- VS Code is not needed generally, but it's needed here because I used Swagger-Editor (https://editor.swagger.io/) to auto-gen the C# server stub and it requires it as a dependency.
- Swagger-Editor also comes in a offline version too you can download to your desktop using Docker.
- See the Swashbuckle project for more notes on how to set this project up.
- 

