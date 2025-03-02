# Unable to click on buttons in the Twilio Blaster

If you’re unable to click on any buttons in the **Twilio Blaster** file, the issue is likely related to macros not being enabled or the file being blocked. Follow these steps to resolve the issue:

**Step 1: Check if the File is Unblocked**

1. Locate the **Twilio Blaster** file on your computer.
2. Right-click on the file and select **Properties**.
3. In the **General** tab, look for a section called **Security** at the bottom.
4. If you see the message "This file came from another computer and might be blocked to help protect this computer," check the box labeled **Unblock**.
5. Click **Apply** and then **OK**.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

**Step 2: Check if You Clicked "Enable Content"**

When opening the file, you should be prompted to "Enable Content". Make sure to click this option. If macros are not enabled, the buttons in the Twilio Blaster will not work.

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

**Step 3: Manually Enabling Macros (if you didn’t receive the prompt)**

If you didn’t receive the "Enable Macros" prompt when opening the file, it could be due to your security settings. Here’s how you can manually adjust the settings:

1. **Open Excel** and click on the **File** tab in the top-left corner.
2. Scroll down and select **Options** from the left-hand menu.
3. In the Excel Options window, click on **Trust Center** from the left panel.
4. Click the **Trust Center Settings** button.
5. In the Trust Center window, select **Macro Settings** from the left panel.
6. You have two options to enable macros:
   * Select **"Disable VBA macros with notification"** – This will prompt you to enable macros each time you open the Twilio Blaster file.
   * Alternatively, select **"Enable VBA macros"** – This will automatically enable macros whenever you open the Twilio Blaster without showing a prompt.
7. Click **OK** to save your changes.
8. Reopen the Twilio Blaster file, and the buttons should now work properly.

{% hint style="info" %}
**Note**: Keep in mind that these are global macro settings. By choosing "Enable VBA macros," macros will automatically run for any Excel file you open, not just the Twilio Blaster. Use this option with caution, especially when working with files from untrusted sources.
{% endhint %}

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
