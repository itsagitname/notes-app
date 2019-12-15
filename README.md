#NotesApp (Grofers Intership Exercise)

Steps to run this application:
Type this commands in the root directory of the application in the Node.js command prompt
-> `npm install` to install all the node modules (dependancies).
-> `npm install -g @aws-amplify/cli` to install all the amplify packages.(This might take a while)
-> `amplify configure` (The following steps are needed to create the backend locally. It won't be needed once the application is deployed.)
    => Select the region as ap-south-1
    => Enter any username of your choice: (user)
    => This will open a IAM management console. Click on Next: Permissions, then click on Next: Tags, next click on Next: Review and finally click on Create user.
    => User is created(See the image below). Copy the Access key and Secret Access Key.
    => Press enter in the command prompt, enter the copied access key and secret access key there. 
    => Finally choose any profile name of your choice(eg: default).
-> `amplify init` to initialize the backend environment
    => Do you want to use an existing environment? No
    => Enter a name for the environment: prod (choose any name)
    => Choose your default editor: Visual Studio Code(choose any editor)
    => Do you want to use an AWS profile? Yes(if you have one already) / No(if you want to make a new one)
    => Please choose the profile you want to use: default(the one which we created in the last step of `amplify configure`)
-> `amplify push`
    => Are you sure you want to continue? (Y/n) y 
    => Do you want to update code for your updated GraphQL API (Y/n) n
    => This might take a while.
-> Finally it is ready to run
    `npm start`
    Runs the app in the development mode.<br />
    Open [http://localhost:3000](http://localhost:3000) to view it in the browser.


These steps might seem to cumbersome to run presently, but this won't be the case after we deploy the full fledged application.
# notes-app
