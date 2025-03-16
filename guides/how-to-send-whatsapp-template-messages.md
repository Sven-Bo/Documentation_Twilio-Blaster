# How to send WhatsApp template messages

{% embed url="https://iframe.mediadelivery.net/play/289332/4e6714d6-7759-49b5-b416-8030b227a672" %}
WhatsApp Template Message Tutorial
{% endembed %}

### What are WhatsApp Template Messages?

WhatsApp template messages are pre-approved message formats that businesses can use to send notifications to customers. They must be approved by WhatsApp before you can use them.

### Setting Up Templates in Twilio

1. **Log in to your Twilio Console**: Go to [Twilio Console](https://console.twilio.com/)
2. **Navigate to WhatsApp Templates**:
   * Go to Develop → Messaging → Content Template Builder
   * Select "Create New Template"
3. **Create Your Template**:
   * Choose a template category (e.g., Marketing, Utility)
   * Write your message content
   * Add variables using the \{{1\}}, \{{2\}} format where you want to personalize the message
   * Submit for approval

For detailed instructions, visit Twilio's official guide: [Creating Templates with the Content Template Builder](https://www.twilio.com/docs/content/create-templates-with-the-content-template-builder)

### Using the WhatsApp Template Sender in Twilio Blaster

#### Step 1: Open the Template Sender Form

* From the main Twilio Blaster interface, click on the "WhatsApp Templates" button
* The WhatsApp Template Sender form will open

#### Step 2: Enter Template ID and Fetch Template

* Enter your Template ID in the input field
* The Template ID looks like: HX94aa222111787f3ddb69f57faa270XXX
* Click the "Fetch" button
* The system will retrieve your template information from Twilio

#### Step 3: Review Template Information

* The template body will be displayed in the preview area
* The template type will be shown (Text, Media, Location, etc.)
* If your template has variables, they will appear in the variable mapping section

#### Step 4: Fill in Template Variables

* For templates with variables, double-click on a variable to edit its value
* You can enter static text or use placeholders in the format \{{PLACEHOLDER\_NAME\}}
* Placeholders will be replaced with data from your recipient list

#### Step 5: Send the Template Messages

* Verify that you have recipients in your Send\_Message sheet
* Click the "Send" button
* Confirm the sending operation when prompted
* The application will send the template message to all your recipients

### Tips for Successful Template Messages

* **Keep templates simple**: Clear, concise messages have higher delivery rates
* **Use variables wisely**: Only use variables for personalization, not for changing the entire message meaning
* **Monitor delivery status**: Check the status column in the Send\_Message sheet after sending

For more help, refer to Twilio's [WhatsApp API documentation](https://www.twilio.com/docs/whatsapp/api)
