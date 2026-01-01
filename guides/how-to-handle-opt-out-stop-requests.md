# How to handle Opt-Out / STOP requests

Twilio Blaster relies on Twilio’s built-in opt-out handling.\
This means STOP requests are handled automatically by Twilio, not by the Excel file.

### How Opt-Out Works with Twilio

Twilio automatically detects common opt-out keywords, including:

* STOP
* STOP ALL
* UNSUBSCRIBE
* CANCEL
* END
* QUIT

When a recipient replies with one of these keywords, Twilio marks the number as opted out at the carrier level. From that moment on, Twilio blocks all outgoing SMS to that number.

This behavior is enforced by Twilio itself and applies to all messages sent through the Twilio API.

Official Twilio documentation:\
[https://help.twilio.com/articles/223134027-Twilio-support-for-opt-out-keywords-SMS-STOP-filtering-](https://help.twilio.com/articles/223134027-Twilio-support-for-opt-out-keywords-SMS-STOP-filtering-)

### What This Means for Twilio Blaster

Twilio Blaster sends messages using the Twilio API.

If a number has opted out:

* Twilio will reject the message automatically
* The message will not be delivered
* The send attempt for that row will fail
* In Twilio Blaster, this appears as a **400 error** in the Status column

You do **not** need to manually remove opted-out numbers before sending. Twilio prevents delivery automatically. That said, you **can** clean up your Excel list manually if you want to avoid seeing failed rows in the Status column. This is optional and only affects how tidy your list looks, not delivery or compliance.

### Recommendation

You have two valid options:

1. **Leave the number in your list**\
   Twilio will block the message and you will see a 400 error for that row. This is expected and confirms opt-out protection is active.
2. **Clean up your list manually**\
   You can remove opted-out numbers if you want a clean send report with fewer failed rows.

Both approaches are fine. Opt-out compliance and message blocking are always handled safely by Twilio.

{% hint style="warning" %}
**Important Note:**  Twilio Blaster does not read incoming replies and does not store opt-out lists inside Excel. All opt-out enforcement happens on Twilio’s side.  This keeps sending simple while staying compliant.
{% endhint %}
