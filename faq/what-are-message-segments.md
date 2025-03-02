# What are message segments?

When sending messages with Twilio Blaster, you’ll notice a **Segments** count in the **Status** column. This helps you understand how your message is split and charged.

<div align="left"><figure><img src="../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure></div>

### What is a Segment?

A **segment** is a portion of your message that fits within a specific character limit before it gets split into multiple parts.

* **Standard SMS (GSM-7 encoding):** Up to **160 characters** per segment.
* **Messages with special characters (UCS-2 encoding, e.g., emojis, certain symbols):** Up to **70 characters** per segment.
* **If your message exceeds these limits, it will be split into multiple segments.**

### Why Does It Matter?

Each segment is counted separately when determining cost and delivery speed. The more segments a message has, the higher the cost.

### Check Your Message Segments

To see how many segments your message will use, try Twilio's official [Message Segment Calculator](https://twiliodeved.github.io/message-segment-calculator/).

For more details on how message segments work, check out Twilio's blog: [What the Heck is a Segment?](https://www.twilio.com/en-us/blog/what-the-heck-is-a-segment-html).
