# How to use the phone number validator

{% embed url="https://iframe.mediadelivery.net/play/289332/fd34a147-2ef6-4574-b77f-ac7884819542" %}
Phonenumber Validator Tutorial
{% endembed %}

### Overview <a href="#overview" id="overview"></a>

The Phone Number Validation & Formatting tool helps you prepare your contact lists for SMS messaging by ensuring all phone numbers are properly formatted and valid. This tool is essential for maximizing your SMS delivery rates and avoiding wasted messages.

### Features <a href="#features" id="features"></a>

* **E.164 Formatting**: Converts phone numbers to the international E.164 format
* **Validation**: Checks if numbers are valid and can receive SMS messages
* **Country Detection**: Determines the country of origin for each number
* **Type Classification**: Identifies whether numbers are mobile, landline, or VoIP
* **Timezone Information**: Shows the timezone associated with each number

### Default Region Setting <a href="#default-region-setting" id="default-region-setting"></a>

The default region setting tells the system which country to use when processing phone numbers without a country code.

**How it works:**

* Numbers with a country code (like +1 or +44) are always processed correctly regardless of your default region
* Numbers without a country code use your selected default region to determine the country

**Examples:**

* If you enter "+1 555-123-4567" → Always formatted as "+15551234567" (US) regardless of default region
* If you enter "555-123-4567" with US as default region → Formatted as "+15551234567"
* If you enter "555-123-4567" with UK as default region → Formatted as "+44555123456"

### How to Use <a href="#how-to-use" id="how-to-use"></a>

1. Enter your phone numbers in the **Input** column
   * Numbers can be in any format (local, with/without country code, with spaces or symbols)
   * Example formats: `(212) 555-1234`, `+44 7700 900123`, `6175550123`
2. Click the **Format & Validate** button
3. Review the results:
   * **Output**: Shows the E.164 formatted number (if valid)
   * **Valid**: Indicates whether the number is valid (Yes/No)
   * **Status**: Shows validation status or error message
   * **Country**: Shows the detected country
   * **Type**: Shows if the number is mobile, landline, or VoIP
   * **Timezone**: Shows the timezone for the number

### Frequently Asked Questions <a href="#frequently-asked-questions" id="frequently-asked-questions"></a>

<details>

<summary>How accurate is the phone number validation?</summary>

The phone number validation uses Google's phone number database to verify if numbers are properly formatted and potentially valid. The tool checks:

* Country code validity
* Number length for the specific country
* Number pattern matching for the region
* Basic structural validity

However, it cannot guarantee with 100% certainty that a number is currently in service or able to receive SMS messages. Only sending a test message can confirm actual deliverability.

</details>

<details>

<summary>Why does a number show as valid but still fail to receive a message?</summary>

A number may be properly formatted and appear valid but still fail to receive messages for several reasons:

* The number may be disconnected or no longer in service
* The subscriber may have blocked  messages
* The number may be a landline that cannot receive SMS/MMS/WhatsApp

</details>

<details>

<summary>Can I validate international numbers?</summary>

Yes! The tool supports phone numbers from virtually all countries worldwide. For best results with international numbers:

* Include the country code with a plus sign (e.g., +44 for UK)
* If the country code is missing, the system will use your selected default region setting

</details>

<details>

<summary>How does the tool handle different number formats?</summary>

The tool is designed to be flexible and can handle most common phone number formats:

* Numbers with spaces, dashes, or parentheses
* Numbers with or without country codes
* Numbers with leading zeros or trunk prefixes

</details>

<details>

<summary>Is there a limit to how many numbers I can validate at once?</summary>

The tool is designed to handle hundreds of phone numbers in a single batch. For very large lists (1000+ numbers), the process may take a bit longer to complete.

</details>

