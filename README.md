
This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).  
  
Below you will find some information on how to perform common tasks.<br>  
You can find the most recent version of this guide [here](https://github.com/facebookincubator/create-react-app/blob/master/packages/react-scripts/template/README.md).  
  
## Pre-Requirements
You need to configure your own GraphQL server or serverless, I recommend using serverless [Graphcool](https://www.graph.cool/) backends, I assume you are already have one.
  
## Get Started  
First clone the project then install the dependencies.
```sh  
    git clone https://github.com/Sh4reef/my-react-relay-starter-kit.git
    cd my-react-relay-starter-kit
    npm install
```  
Next you need to install [get-graphql-schema](https://www.npmjs.com/package/get-graphql-schema) globally, We use this to get `schema.graphql` file from GraphQL API endpoint, Here I used my GraphQL API endpoint for demonstration.
```sh
	npm install -g get-graphql-schema
	get-graphql-schema https://api.graph.cool/relay/v1/sh4reef > ./schema.graphql
```
  You should see `schema.graphql` file inside `my-react-relay-starter-kit` folder.
  


----------
Start the app
```sh
npm run start
```
Then open [http://localhost:3000/](http://localhost:3000/) to see your app.<br>  
When you’re ready to deploy to production, create a minified bundle with 
```sh
npm run build
```