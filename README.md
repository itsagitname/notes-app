# NotesApp (Grofers Internship Exercise)

Steps to run this application: <br />
Type this commands in the root directory of the application in the Node.js command prompt <br />
-> `npm install` to install all the node modules (dependancies). <br />
-> `npm install -g @aws-amplify/cli` to install all the amplify packages.(This might take a while) <br />
-> `amplify configure` (The following steps are needed to create the backend locally. It won't be needed once the application is deployed.) <br />
  &nbsp; => Select the region as ap-south-1 <br />
  &nbsp;  => Enter any username of your choice: (user) <br />
  &nbsp; => This will open a IAM management console. Click on Next: Permissions, then click on Next: Tags, next click on Next: Review and finally click on Create user. <br />
  &nbsp; => User is created(See the image below). Copy the Access key and Secret Access Key. <br />
  &nbsp;  => Press enter in the command prompt, enter the copied access key and secret access key there. <br />
  &nbsp;  => Finally choose any profile name of your choice(eg: default). <br />
-> `amplify init` to initialize the backend environment <br />
  &nbsp;  => Do you want to use an existing environment? No <br />
  &nbsp; => Enter a name for the environment: prod (choose any name) <br />
  &nbsp;  => Choose your default editor: Visual Studio Code(choose any editor) <br />
  &nbsp;  => Do you want to use an AWS profile? Yes(if you have one already) / No(if you want to make a new one) <br />
  &nbsp;  => Please choose the profile you want to use: default(the one which we created in the last step of `amplify configure`) <br />
-> `amplify push` <br />
  &nbsp;  => Are you sure you want to continue? (Y/n) y  <br />
  &nbsp;  => Do you want to update code for your updated GraphQL API (Y/n) n <br />
  &nbsp;  => This might take a while. <br />
-> Finally it is ready to run <br />
  &nbsp;  `npm start` <br />
    Runs the app in the development mode.<br /> 
    Open [http://localhost:3000](http://localhost:3000) to view it in the browser. <br />


These steps might seem to cumbersome to run presently, but this won't be the case after we deploy the full fledged application.
# notes-app
