# How to send MMS

{% hint style="info" %}
### Country and Carrier Limitations

**Important**: MMS messages are supported only in the following countries:

* **United States**
* **Canada**
* **Australia**

MMS can only be sent to carriers that support MMS in these countries. Unsupported carriers will convert MMS into an SMS with a short URL link (if MMS Converter is enabled). For more details, see [Getting Started with MMS Converter](https://help.twilio.com/articles/360032795214-Getting-Started-with-MMS-Converter).

Below is an example image of how an MMS with a short URL will appear **if MMS is not available**:

![](<../.gitbook/assets/image (10).png>)
{% endhint %}

### How to Send MMS

To send an MMS message, use the "Image URL" column in your Excel file. If you do not wish to send an MMS, leave this cell blank. Follow the notes below for successful MMS sending:

#### Requirements for Sending MMS

1. **Supported File Types**: `.gif`, `.png`, `.jpeg`. Unsupported formats will be rejected.
2. **File Size Limit**: Each media file must not exceed **5 MB**.
3. **Valid URLs Only**: The URL should directly display the file.
   * ✅ **Example**: `https://demo.twilio.com/owl.png`
   * ⛔ **Invalid**: `C:\Users\Username\Desktop\cat.jpg`
4. **Multiple Images**: Separate multiple image URLs using a semicolon (`;`).
   * **Example**: `https://demo.twilio.com/owl1.png;https://demo.twilio.com/owl2.png`
5. **File Location**: Host the files online (e.g., Dropbox, Google Drive, or your own web server) and ensure the URL links directly to the file.

**Example for Google Drive:**

1. Go to your Google Drive and right-click on the image file.
2. Select **Share** and enable **Anyone with the link**.
3. Copy the file ID from the URL (e.g., `1wMgCWAsqlw0nXcMhCldTbwSznMdXUmBT`).
4. Use the following format to create a direct link:
   * `https://drive.google.com/uc?id=FILE_ID`
   * ✅ **Result**: `https://drive.google.com/uc?id=1wMgCWAsqlw0nXcMhCldTbwSznMdXUmBT`

#### Using the MMS Link Converter

To save time, you can use the **MMS Link Converter** tool built into Twilio Blaster.

* Just paste your **Google Drive** or **Dropbox** sharing link into the tool, and it will generate a direct link for you.

**Example for Google Drive:**

* ❌ Shared Link:\
  `https://drive.google.com/file/d/1wMgCWAsqlw0nXcMhCldTbwSznMdXUmBT/view?usp=sharing`
* ✅ Direct Link:\
  `https://drive.google.com/uc?id=1wMgCWAsqlw0nXcMhCldTbwSznMdXUmBT`

**Example for Dropbox:**

* ❌ Shared Link:\
  `https://www.dropbox.com/s/abcd1234/myfile.png?dl=0`
* ✅ Direct Link:\
  `https://www.dropbox.com/s/abcd1234/myfile.png?raw=1`

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>MMS Link Converter Tool</p></figcaption></figure>

How to Fill the Image URL Column

* Enter the full URL of the image in the "Image URL" cell for the corresponding message row.
* Ensure the URL is accessible and hosted online. Invalid URLs will be flagged in the "Status" column with an error message.

***

### Example

Here is an example configuration for sending an MMS:

| Receiver Number | Text Message         | Image URL                                                                                                                              | Status                      |
| --------------- | -------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| +1234567890     | Check out this owl!  | [https://demo.twilio.com/owl.png](https://demo.twilio.com/owl.png)                                                                     | Sent successfully           |
| +0987654321     | Here are two owls!   | [https://demo.twilio.com/owl1.png;https://demo.twilio.com/owl2.png](https://demo.twilio.com/owl1.png;https://demo.twilio.com/owl2.png) | Sent successfully           |
| +1123456789     | Missing file example | C:\Users\Username\Desktop\cat.jpg                                                                                                      | Skipped - Invalid Media URL |

***

### Recommendations for File Names

When hosting your images, follow these guidelines for file names:

1. Avoid using spaces or special characters (`~ ! @ # $ % ^ & * ( ) [ ] { }`).
2. Keep the file name under 20 characters.
3. Example:
   * ✅ `owl.png`
   * ⛔ `my owl picture!.jpg`

***

### Additional Information

For more details on sending and receiving MMS messages with Twilio, visit their official documentation: [Twilio MMS Guide](https://help.twilio.com/articles/223179808-Sending-and-receiving-MMS-messages).
