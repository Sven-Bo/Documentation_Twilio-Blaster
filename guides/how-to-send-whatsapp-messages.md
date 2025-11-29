# How to send WhatsApp messages

To send WhatsApp messages using Twilio Blaster, follow these simple steps:

1. **Enable WhatsApp Messaging**: In the settings, set the WhatsApp messaging option to "On".\
   ![](<../.gitbook/assets/image (1) (1) (1).png>)
2. **Set Up a WhatsApp API Number**: You'll need a WhatsApp-enabled phone number. This involves registering your number through Twilio. Detailed instructions are available in Twilio's guide: \
   👉 [**\[Twilio\] Register on WhatsApp using Self Sign-up**](https://www.twilio.com/docs/whatsapp/self-sign-up)
3. **Sending Messages**: Once set up, you can send text messages as usual.
4. **Sending Images**: To include an image, provide the media URL in the "Image URL" column. This process is similar to sending an MMS. Note that WhatsApp messages via Twilio allows **only one image per message**. For more details, refer to the MMS guide: [#how-to-send-mms](how-to-send-mms.md#how-to-send-mms "mention")

{% hint style="info" %}
Aside from enabling WhatsApp and setting up the API number, the process remains the same as sending regular messages. This means you can also schedule WhatsApp messages.
{% endhint %}
