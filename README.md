# CodeComp3-Java-Player

## Prerequisites to play
- Git
- Editor of your choice(eclipse/intelliJ recommended)

## How to play from your local machine with 'dumb' algo
We have written all boilerplate code to get you started within 5 minutes. You kust need to make 'MySmartAlgo' smarter. You can improve your algo by playing with test server.
- Clone this repo using : git clone <Link of this repo>
- cd codecomp3-java-player
- change 'myTeam' and 'pass' in application.properties inside src/main/resources
- Using editor of your choice, Run as Java Application or as maven project using run goal as : clean spring-boot:run and start playing.
- see url for live score : <leaderboard URL Here>

## Final Competition Day
- You need to deploy your algo in Google Cloud Platform to connect to game server.
- Fork this repository, modify algo, add team name and password in src/main/resources/application.properties file,check-in and deploy into Google Cloud from your github repository.
-  Step-by-step guide to deploy a Java application on google cloud is given below:

## Step-by-step guide

1. Visit the codecomp team's [repo](https://github.com/ayu004/gcp-infra-codecomp) to setup the google cloud infrastructure to deploy bot on.
  - Link to Repo : https://github.com/ayu004/gcp-infra-codecomp

2. Add the 2 github secrets(PROJECT_ID and GOOGLE_APPLICATION_CREDENTIALS) to this forked repository of yours, as was done in the repository used to create infrastrucre in step 1.

#### Now you are good to go, whenever you push anything to your repo's master branch it will get deployed to Google App Engine of your GCP Project using Github Actions.
 - Whenever you push to master branch you can see your Github Action Running in Actions tab. Wait for it to complete as shown in image below

 ![Github Action Running](/assets/gae-deploy-github-action.png)
 
 - Your bot is now deployed on google cloud. You can go ahead and check the logs

3. Checking Logs
  - Go to App Engine > Services and click on Tools in your default deployed service and select Logs which will open the logs of application.
  - You can click on Play button on top to start streaming live logs.

![Logs](/assets/logs.PNG) 

- It might take some time to service to get up and running or logs to load initially

## Happy Coding :smile:  



