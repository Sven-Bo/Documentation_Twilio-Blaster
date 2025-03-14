# How to use placeholders

{% embed url="https://iframe.mediadelivery.net/play/289332/d65deb5b-9f40-46d9-894c-91556331db73" %}
Watch the placeholder tutorial
{% endembed %}

#### What Are Placeholders? <a href="#what-are-placeholders" id="what-are-placeholders"></a>

Placeholders are special tags in your messages that get replaced with real information when you send your message. They make your messages more personal and relevant to each recipient.

#### How Placeholders Work <a href="#how-placeholders-work" id="how-placeholders-work"></a>

* Placeholders use double curly braces: `{{placeholder_name}}`
* When you send a message, the system automatically replaces these tags with the actual values
* Example: "Hello \{{first\_name\}}" becomes "Hello John" when sent to John

#### Types of Placeholders <a href="#types-of-placeholders" id="types-of-placeholders"></a>

**Global Placeholders**

These work for all recipients and are replaced with the same value for everyone.

Examples:

* `{{company_name}}` - Your business name
* `{{today}}` - Current date
* `{{offer_code}}` - Promotion code for everyone

**Number-Specific Placeholders**

These are unique to each recipient and change based on who receives the message.

Examples:

* `{{first_name}}` - Recipient's first name
* `{{last_name}}` - Recipient's last name
* `{{appointment_date}}` - Specific appointment for this person

#### Using Fallback Values <a href="#using-fallback-values" id="using-fallback-values"></a>

If you're not sure a placeholder has a value, you can add a fallback using the pipe symbol (|).

Example: `{{first_name|Friend}}`

* If first\_name exists: "Hello John"
* If first\_name is empty: "Hello Friend"

#### Placeholder Resolution Flow <a href="#placeholder-resolution-flow" id="placeholder-resolution-flow"></a>

When processing your message, the system replaces placeholders in this order:

1. **Number-Specific Placeholders**: Checked first and have the highest priority
2. **Global Placeholders**: Used if no matching number-specific placeholder is found
3. **Fallback Values**: Used if neither number-specific nor global values are available
4. **Empty String**: If no value is found and no fallback is provided, the placeholder is removed

This means if you have the same placeholder name in both number-specific and global settings, the number-specific value will be used.

#### How to Set Up Placeholders <a href="#how-to-set-up-placeholders" id="how-to-set-up-placeholders"></a>

1. Go to the Placeholders sheet
2. The table has two types of rows:
   * **global**: For placeholders that apply to all messages
   * **number-specific**: For placeholders that are unique to specific phone numbers
3. For global placeholders:
   * Set Type column to "global"
   * Leave Phone Number column empty
   * Add your placeholder tags and values in the pairs of columns
4. For number-specific placeholders:
   * Set Type column to "number-specific"
   * Enter the specific phone number in E.164 format (e.g., +15551234567)
   * Add your placeholder tags and values in the pairs of columns

#### Tips for Using Placeholders <a href="#tips-for-using-placeholders" id="tips-for-using-placeholders"></a>

* Always test your messages before sending to many people
* Use the "Add Samples" button to see how placeholders work
* Remember that number-specific placeholders need the exact phone number in E.164 format
* Number-specific placeholders take priority over global ones with the same name

#### Common Questions

<details>

<summary>What happens if a placeholder doesn't have a value</summary>

The system follows the resolution flow: number-specific → global → fallback → empty string. If no value is found at any step, the placeholder is replaced with an empty string.

</details>

<details>

<summary>How many placeholders can I use in one message?</summary>

You can use as many as you need, but remember that messages have character limits.

</details>

<details>

<summary>Can I use the same placeholder name for both global and number-specifc</summary>

Yes. In this case, the number-specific value will be used for that recipient, while others will get the global value.

</details>

