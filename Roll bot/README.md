A Roll bot for Slack
===============================

Use the roll bot to roll a dice on slack. It is developed with incoming webhooks and slash commands, in NodeJs.
Roll bot is perfect for DnD campaigns or just for some fun, I personally developed it for the former.

=======
Please see below for a tutorial on how to set up the Roll bot.


First - We need to set up slash command integration so that we can send signals to our bot by using the /roll command. To do this you need to go to your integrations and search for a slash command integration
![Alt tag](https://github.com/sqiggg/Slack-Bot/blob/master/Roll%20bot/tutorial_images/slash_intergrations.png?raw=true "Slash Integration")


Next - Choose the name of your command - I suggest /roll but really you can use anything.
![Alt tag](/tutorial_images/choose_command.png?raw=true "Choosing a Command")


Then - Set up the finer points of the Slash command: pay attention to the fact that the web address needs to be on port 3000 because thats the port that we're listening to. Also make sure that you set your method to POST not GET.
![Alt tag](/tutorial_images/slash_settings.png?raw=true "Configuring Slash commands")

After you've done that, we can move on to setting up the incoming webhook. To do this we need to again search for an integration, but this time we need to search for incoming webhook.
![Alt tag](/tutorial_images/incoming_webhook.png?raw=true "Searching for the Incoming Webhook integration")

Next we need to setup the incoming webhook integration. The important bit here is that we need to get the url and put it into the path variable that is located in the send function near the bottom of dicebot.js.
![Alt tag](/tutorial_images/ow_settings.png?raw=true "Configuring the incoming webhook")


Thats it now heres the end product:
![Alt tag](/tutorial_images/the_end_command.png?raw=true "It works :)")


Thank you everyone for reading and I hope that this works for you. Please leave suggestions as this is my first github repo.
