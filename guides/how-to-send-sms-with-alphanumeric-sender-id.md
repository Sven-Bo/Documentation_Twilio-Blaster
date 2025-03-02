# How to send SMS with Alphanumeric Sender ID

### What is an Alphanumeric Sender ID?

An Alphanumeric Sender ID lets you send SMS messages using your **brand name** or **company name** as the sender instead of a phone number.

The example below shows how an Alphanumeric Sender ID (_AUTHMSG)_ would look in place of the standard number.&#x20;

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

**Key Benefits:**

* Great for branding.
* Easy to recognize by your recipients.

**For details, see Twilio’s official guide:**

👉 [Getting started with Alphanumeric-Sender-ID](https://help.twilio.com/articles/223181348-Getting-started-with-Alphanumeric-Sender-ID)

***

### How to Use an Alphanumeric Sender ID in Twilio Blaster?

{% stepper %}
{% step %}
### Check Support for Your Country:

Not all countries allow Alphanumeric Sender IDs. Some require registration.\
Check the list of supported countries here:\
[Twilio Supported Countries](https://help.twilio.com/articles/223133767-International-support-for-Alphanumeric-Sender-ID).
{% endstep %}

{% step %}
### Enable or Register Your Sender ID in Twilio (if required):

* Go to the Twilio Console.
* Navigate to **Phone Numbers > Alphanumeric Sender ID** and register your ID if required.
* For help, follow Twilio’s guide:\
  [How to Register an Alphanumeric Sender ID](https://help.twilio.com/articles/20153208099611-How-to-Register-an-Alphanumeric-Sender-ID).
{% endstep %}

{% step %}
### Input the Sender ID in Twilio Blaster:

* In the **From Number** cell, enter your Alphanumeric Sender ID.\
  &#xNAN;_(Example: `MyBrand` or `Company123`)_
*

    <figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="info" %}
**Key Requirements  for your Alphanumeric Sender ID.:**

* 3 to 11 characters long.
* Must include at least one letter.
* Cannot include special characters (e.g., #, @, %, etc.).
{% endhint %}

***

### Frequently Asked Questions (FAQ)

**Q: Does this work with MMS?**\
A: Alphanumeric Sender IDs are supported for **SMS only**, not MMS. If you need to send MMS, you must use a phone number instead.

**Q: I inputted my Sender ID, but I see "Invalid 'From' Number" in the status column when sending. Why?**\
A: Ensure your Sender ID follows the **requirements**:

* It must be 3 to 11 characters long.
* It must include at least one letter.
* It cannot include special characters.
