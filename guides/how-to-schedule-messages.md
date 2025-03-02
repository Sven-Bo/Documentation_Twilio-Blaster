# How to schedule messages

#### 1. Set Up a Messaging Service

A Messaging Service in Twilio groups your sending channels (like phone numbers and WhatsApp senders) into one container, making it easier to manage messages. **Without a Messaging Service, scheduling messages isn't possible**.

* **How to Create a Messaging Service:**
  * Log in to your Twilio account.
  * Navigate to the [Messaging Services](https://www.twilio.com/console/sms/services) section.
  * Click "Create Messaging Service" and follow the prompts.
  * For detailed guidance, refer to Twilio's [Getting Started with Messaging Services](https://help.twilio.com/articles/223181308-Getting-started-with-Messaging-Services).

**Example Video:**\
Here is a sample video on how to set up a Messaging Service. Keep in mind that this is just an example—you might need to adjust it based on your needs.

{% embed url="https://iframe.mediadelivery.net/play/289332/b51eeb24-f6af-4e50-8af6-1689d4fd4d26" %}
Twilio Messaging Service Demo Setup
{% endembed %}



***

#### 2. Schedule Messages Using UTC

When scheduling a message, you must enter the send time in Coordinated Universal Time (UTC).

* **What is UTC?**\
  UTC is the global time standard. Unlike local time zones, it stays the same worldwide, ensuring messages are sent at the correct time, no matter where you or your recipients are.
* **How to Convert Local Time to UTC:**\
  If you're unsure what UTC time to use, you can convert your local time with my [UTC Converter Tool](https://pythonandvba.com/go/twilio-blaster-utc-converter).
* **Scheduling Limits:**
  * Messages must be scheduled at least **15 minutes** in advance.
  * You can schedule messages up to **35 days** in advance.

Once you've set up a Messaging Service and entered the scheduled send time in UTC, Twilio Blaster will handle the rest.
