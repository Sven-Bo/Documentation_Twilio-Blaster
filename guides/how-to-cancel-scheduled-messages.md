# How to cancel scheduled messages

{% hint style="info" %}
To cancel a scheduled message, you **must** have the **Message ID**. Enter it in the **Message ID** column to proceed.

If you don't know the **Message ID**, you can retrieve it from the Twilio messaging logs: [View Messaging Logs](https://pythonandvba.com/go/twilio-blaster-messaging-logs).
{% endhint %}

### Tutorial Video

Watch this  video to see how to cancel scheduled messages (works for SMS, MMS, and WhatsApp):

{% embed url="https://iframe.mediadelivery.net/play/289332/b570f6f7-7e1a-4837-86b1-46f4e96f48e3" %}
How to cancel scheduled messages
{% endembed %}

### Steps to cancel scheduled messages

1. **Enter the Message ID**
   * If you still see your scheduled messages in the list, the **Message ID** should already be there.
   * If you cleared your message list, retrieve the **Message ID** from your Twilio logs and paste it into the **Message ID** column.
2. **Cancel the Scheduled Message**
   * Click the **Cancel Scheduled Messages** button.
   * Twilio Blaster will go through each row, check for a **Message ID**, and attempt to cancel it.
   * No need to filter for scheduled messages—Twilio Blaster will attempt to cancel every message with an ID.
3. **Check the Status**
   * If a message **cannot** be canceled (e.g., it has already been delivered), the **Status** column will update accordingly.
   * Click **Refresh Status** to confirm which messages were successfully canceled.
