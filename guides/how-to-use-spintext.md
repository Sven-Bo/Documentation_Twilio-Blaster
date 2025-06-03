---
description: >-
  Ever wish your messages didn’t sound like they were copied and pasted a
  hundred times over? That’s where spintext comes in.
---

# How to use spintext

#### What is spintext? <a href="#what-is-spintext" id="what-is-spintext"></a>

Spintext is a simple way to make your messages feel more human by adding variation. You define different versions of a word or phrase, and the tool randomly picks one each time the message is sent.

Here’s the basic format:

Copy

```
[[Hi|Hello|Hey]] Sarah, just checking in!
```

**Possible output:**

> Hello Sarah, just checking in!

Every time a message goes out, one of those options is chosen at random. That way, even if the message content stays the same, it doesn’t _feel_ the same.

***

#### Using spintext with placeholders <a href="#using-spintext-with-placeholders" id="using-spintext-with-placeholders"></a>

Spintext works perfectly with placeholders like `{{FirstName}}` or `{{Company}}`.

You can even nest placeholders inside spintext:

Copy

```
[[Hi {{FirstName}}|Hello {{FirstName}}|Hey there]]
```

**Possible output:**

> Hey there

or

> Hello Alex

This way, your message gets personalized _and_ varied—without extra work.

***

#### A few tips <a href="#a-few-tips" id="a-few-tips"></a>

* Use `[[ ]]` for spintext blocks
* Separate options with `|` (the pipe symbol)
* You can include as few or as many options as you want
* `[[]]` (an empty block) just disappears in the final message
* Each block is handled separately, even if there are multiple in the same message

***

#### FAQ <a href="#faq" id="faq"></a>

<details>

<summary><strong>What happens if I only put one item inside the brackets?</strong></summary>

It’ll just use that item—no randomization happens.

</details>

<details>

<summary><strong>Can I put spintext inside another spintext block?</strong></summary>

Nope. Nested spintext like `[[option1|[[nested1|nested2]]]]` isn’t supported. It’ll be ignored.

</details>

<details>

<summary><strong>Can I add emojis, punctuation, or full sentences?</strong></summary>

Absolutely. You can spin whole phrases if you like:

```
[[Thanks a lot!|Appreciate it.|Much obliged!]]
```

</details>

<details>

<summary><strong>Will it choose a different result every time?</strong></summary>

Yes—each message sent will process the spintext anew, picking random options independently.

</details>

#### Final thought <a href="#final-thought" id="final-thought"></a>

Spintext is a small trick with a big impact. Think of it like changing your tone when speaking to different people—it keeps things friendly, personal, and just a little more human.

Give it a try and see how your messages start feeling less like broadcasts, and more like conversations.
