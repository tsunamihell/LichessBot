# LichessBot
Very easy way to make a lichess bot

Create your own permanent Lichess BoT

If you want to create your own permanent bot, do the following:

Sign up to GitHub https://github.com/join , if you have not already.

With your GitHub account  click on Fork.

Create a BOT account if you do not already have one. To create one use an account that has not played any games yet, log into this account, then visit https://hypereasy.herokuapp.com/auth/lichess/bot , approve oauth and then on the page you are taken to click on 'Request upgrade to bot'. 

Create an API access token with your BOT account at https://lichess.org/account/oauth/token/create?scopes[]=challenge:read&scopes[]=challenge:write&scopes[]=bot:play&description=Hyper%20Bot%20TOKEN ( should have scopes Read incoming challenges / Create, accept, decline challenges / Play games with the bot API )

Sign up to Heroku https://signup.heroku.com/ , if you have not already.

At Heroku create a new app using New / Create new app. Choose Europe for region.

In the app's dashboard go to the Deploy tab. Use the GitHub button to connect the app to your forked repo. Press Search to find your repositories, then select LichessBot. You need to deploy the master branch. Enable Automatic Deploys and press Deploy Branch, for the initial deploy. Wait for the build to finish.

In Heroku Settings / Reveal Config Vars create a new variable TOKEN and set its value to your newly created access token, then create a new variable BOT_NAME and set its value to your bot's lichess username.


Congratulations, you have an lichess bot which is playing!

**NOTICE**
Your bot maybe not online sometimes because it will be sleeping
If your bot stops playing restart your dynos by clicking on more and then restart dynos and wait for 1min
It will play variants but it will be weak
