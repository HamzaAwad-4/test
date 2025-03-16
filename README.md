IP Grabber
Inspiration from ipgrabber by baum1810
Made with ❤️ by John Wick.
Add me on Discord - JohnWick#0001. Happy tracking!

📨 IP Logger with Discord Webhook
Tired of 429?:
This IP logger uses Discord webhooks to send data to a specified Discord channel. Instead of using a persistent webhook, the application creates a new webhook, sends the data, and then deletes it for each request. This approach is adopted to bypass Discord's rate limiting, which restricts the number of requests a client can make within a certain period. Rate limiting prevents spamming or overloading Discord's API. Thanks to our create-send-delete process, you can enjoy smooth and uninterrupted IP logging without worrying about hitting rate limits! 🚀

💬 Frequently Asked Questions (FAQs)
Click to expand
Table of Contents
🚀 Deployment
🔒 Environment Variables
⚙️ Customization
🛠️ Debugging and Logging
💡 Ideas for Extending the Project

🚀 Deployment
Click the Deploy button below to get started. All the work has been done for you! However, if you want to avoid an unnecessary headache, continue reading into the next instructions!

During the deployment setup process, you'll need to add the required environment variables as explained in the Environment Variables section. Note: See Enviornmental Variables in the next section for clarity!

After adding the environment variables, click "Deploy" to deploy your project.

Deploy with Vercel


Click to see pictures and clear instructions if you don't know what you are doing!
🔒 Environment Variables
Before deploying the application, you need to provide some environment variables. To do this, follow these steps during the deployment setup process shown in the GIF above:

Scroll down to the "Environment Variables" section.
Add the following variables:
channel_id: Your Discord channel ID where the webhook should send messages.
bot_token: Your Discord bot token for creating and managing webhooks.
ip_token: Your IPinfo.io API token for fetching IP address information.
redirect_url: The URL where users will be redirected at log completion.
By storing these variables in the Vercel dashboard, you prevent exposing sensitive information and make it easier to manage the variables across different environments (e.g., development, staging, and production).

When you update the values of the environment variables in the Vercel dashboard, they will automatically be applied to your application without the need to modify your code.

Read more about Vercel's Environment Variables for best practices and usage.


⚙️ Customization
You can customize various aspects of your IP Logger to create a unique and personalized experience. Here are some ideas:

Click to expand

🛠️ Debugging and Logging
When adding new features or customizing the application, you might encounter issues or errors. To help with troubleshooting and debugging, you can enable logging in your Vercel application.

  1. In your Vercel project dashboard, go to the Settings tab.
  2. Navigate to the Environment Variables section.
  3. Add a new environment variable with the key LOG_LEVEL and a value of debug. This will enable detailed logging in your application.

After setting the LOG_LEVEL environment variable, redeploy your application for the changes to take effect.

To view the logs, go to the Deployments tab in your project's Vercel dashboard, click on the desired deployment, and then click on the Functions tab. Here, you can select a function to view its logs.

When you're finished debugging, you can remove or change the LOG_LEVEL environment variable to a lower verbosity level (e.g., info, warn, or error) to reduce the log output.

Note: Be cautious when sharing logs, as they may contain sensitive information.


💡 Ideas for Extending the Project
Click to expand

Made with ❤️ by John Wick.
Add me on Discord - JohnWick#0001. Happy tracking!
