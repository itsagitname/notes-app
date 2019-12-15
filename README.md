# NotesApp (Grofers Intership Exercise)

Steps to run this application: <br />
Type this commands in the root directory of the application in the Node.js command prompt <br />
-> `npm install` to install all the node modules (dependancies). <br />
-> `npm install -g @aws-amplify/cli` to install all the amplify packages.(This might take a while) <br />
-> `amplify configure` (The following steps are needed to create the backend locally. It won't be needed once the application is deployed.) <br />
    => Select the region as ap-south-1 <br />
    => Enter any username of your choice: (user) <br />
    => This will open a IAM management console. Click on Next: Permissions, then click on Next: Tags, next click on Next: Review and finally click on Create user. <br />
    => User is created(See the image below). Copy the Access key and Secret Access Key. <br />
    => Press enter in the command prompt, enter the copied access key and secret access key there. <br />
    => Finally choose any profile name of your choice(eg: default). <br />
-> `amplify init` to initialize the backend environment <br />
    => Do you want to use an existing environment? No <br />
    => Enter a name for the environment: prod (choose any name) <br />
    => Choose your default editor: Visual Studio Code(choose any editor) <br />
    => Do you want to use an AWS profile? Yes(if you have one already) / No(if you want to make a new one) <br />
    => Please choose the profile you want to use: default(the one which we created in the last step of `amplify configure`) <br />
-> `amplify push` <br />
    => Are you sure you want to continue? (Y/n) y  <br />
    => Do you want to update code for your updated GraphQL API (Y/n) n <br />
    => This might take a while. <br />
-> Finally it is ready to run <br />
    `npm start` <br />
    Runs the app in the development mode.<br /> 
    Open [http://localhost:3000](http://localhost:3000) to view it in the browser. <br />


These steps might seem to cumbersome to run presently, but this won't be the case after we deploy the full fledged application.
# notes-app
