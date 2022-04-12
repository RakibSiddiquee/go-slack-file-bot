## Golang Slack File Bot

1. Create a new app name "file-bot" entering into the url https://api.slack.com/apps  
2. Create a socket-token in App-Level Tokens under Basic Information
3. Go to OAuth & Permissions menu and add the following scopes:  
channels:read  
chat:write  
files:read  
files:write  
im:read  
mpim:history  
remote_files:read  
remote_files:share  
remote_files:write  

4. Then, click on the button 'Install to Workspace' under OAuth Tokens for Your Workspace and click on the allow button  

5. After that copy the Bot User OAuth Token and paste it into the set env SLACK_BOT_TOKEN inside main function in main.go  

6. Copy the channel id by right clicking on general channel -> open channel details and paste in paste it into the set env CHANNEL_ID inside main function in main.go  

Install the package:  
1. https://github.com/slack-go/slack


Finnaly add the file-bot into the channel and run the following command:  
1. go build
2. go run main.go