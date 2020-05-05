# TelegramBot
A simple telegram bot which returns the same message you type in telegram and sends to your bot

There are 2 ways to get update from telegram server:
1. Long Polling
2. Setting WebHooks

We will be using webhooks method.

Below are the steps which will help you create the simple bot. 

1. Register a bot in Telegram's @BotFather using /newbot.
2. Create an AWS account and create an API in API Gateway.
3. Create a function in AWS Lambda.
4. Connecting lambda function to our API.
    1. Create a method in resource in the API and insert the lambda function where prompted.
    2. Click save and deploy API.
    3. Now we have a secure URL to out lambda function.
5. Setting webhooks
    1. Type the below URL in your browser with you BOT TOKEN AND API URL.
       https://api.telegram.org/bot<your-bot-token/setWebHook?url=your-API-invoke-URL
    2. You will receive a confirmation message from telegram.
    3. Write the code in the lambda function visual editor.
        1. The code only defines to fetch the message sent to the bot and it resends the same message to the bot.
6. Test your application by sending message to your bot.


Note: This is just a brief description for creating a telegram bot which i have used for my purpose in order to revisit in future.
If any of you wishes to clarify any of your doubt you are welcome with all your doubts.

Happy CoDing :)
 
     
