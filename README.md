# The Standup and Prosper FAQ
Below are listed some common answers for a few more complex activities in S&P

#### Filling out the standup
* [How to paste formatted markdown into report dialog?](#q-how-to-paste-formatted-markdown-into-report-dialog)
* [How to stop the bot from mentioning users?](#q-how-to-stop-the-bot-from-mentioning-users)
* [What are the Standup & Prosper hidden commands?](#q-what-are-the-standup--prosper-hidden-commands)

#### Configuration
* [How to make standups aware of the user's timezone?](#q-how-to-make-standups-aware-of-the-users-timezone)
* [The owner of the standup is no longer part of the Slack workspace.](#q-the-owner-of-the-standup-is-no-longer-part-of-the-slack-workspace)
* [How to improve replies to the standup report?](#q-how-to-improve-replies-to-the-standup-report)

#### Advanced Options
* [What does the report portal look like?](#q-what-does-the-report-portal-look-like)
* [How to set a reminder on Friday for a Monday standup?](#q-how-to-set-a-reminder-on-friday-for-a-monday-standup)
* [Why was the standup 5 minutes late?](#q-why-was-the-standup-5-minutes-late)

#### Related to this FAQ
* [I can't find an answer to my question.](#q-i-cant-find-an-answer-to-my-question)

## Q: I can't find an answer to my question?
Click [Create a new issue](https://github.com/Teaminator/Standup-and-Prosper-FAQ/issues/new) and ask away, or if you figured out something that you want everyone to know, just click [edit the FAQ](https://github.com/Teaminator/Standup-and-Prosper-FAQ/edit/main/README.md). (You'll need an [github.com](https://github.com) account for this). If neither of those are options that work for you, send an email to the [Standup Support DL](mailto:faq-support@teaminator.io).

## Q: How to improve replies to the standup report?
There are two options for how to post the standup report.

![image](https://user-images.githubusercontent.com/5056218/145066466-1f7031b9-d624-4ecd-9d78-479cf1b5da78.png)
* Posting the report **directly to the channel** makes it possible to reply to individual questions or to team members.
* Sending the report **to a thread** is great for channels with lots of communication and prevents disruptions

Unless your channel is one that has more than 20 people in it, Standup & Prosper recommends posting directly to the channel.

![image](https://user-images.githubusercontent.com/5056218/145067470-f826f9ca-8054-4138-8882-eaaa0932ebb1.png)

Threaded responses are hidden in the thread:

![image](https://user-images.githubusercontent.com/5056218/145558763-f18a8e37-6a50-4c81-b587-c38e5e3871d8.png)

## Q: What does the report portal look like?
![standup-report-image](https://user-images.githubusercontent.com/5056218/147956686-a827b1f6-9a1a-4c98-bf1b-5339f35acadd.png)

## Q: How to paste formatted markdown into report dialog?
The standup popup dialog doesn't allow preformatted text, even though we have requested from Slack to allow this multiple times. There is just no way to support it, these fields only support markdown.

#### Why is preformatted even necessary?

In some cases standup team members may want to copy their previous day's standup answers to today. In those cases rather than manually copying and pasting, there is a great automated solution that exists to solve this problem. Just enable the **Autofill prepopulation** and Standup & Prosper will take care of the rest. Answers will be automatically populated into the dialog the next day **in markdown**, making it easy for your team members to edit their responses.

![image](https://user-images.githubusercontent.com/5056218/145195899-ed573dfd-c55e-426a-af2e-19ab0b069a28.png)

#### I still want preformatted text
That's no problem, preformatted text can already be pasted directly to the bot in a standup conversation. Just take the response and paste it directly in the chat box. What you see here is what Standup & Prosper will send back to the team at report time.

![image](https://user-images.githubusercontent.com/5056218/145196748-ca6fe163-5a85-4c50-98da-5d854c091b05.png)

## Q: How to make standups aware of the user's timezone?
A common question about scheduling is "I want to have every user in the standup get reminded at 10:00AM in their timezone to answer the standup, how do I do this?". Great, the best way to achieve this for your team is to create one standup in each of the timezones where the users are, and assign just the users to that standup. It might seem that it would be better to have a single standup, which has a single report time, however that's actually not the best pattern.

Let's take a look at some common problems that the multi-standup approach solves. For this, we'll assume there is one team in EST (UTC-4) and one team in IST (UTC+5.5):
* If the report time is at 5PM EST--then IST enters their standup at 10AM IST, but the report happens at 2:30AM IST that's not valuable for that team that has to wait 24 hours until they are in the office the next day to see the standup of their own team members. Likewise, the team in EST, also is waiting until the next day.
* If the report time is at 12PM EST--then IST enters their standup at 10AM IST, but the report happens at 9:30PM IST. That fixes the problem for EST but not IST.

Commonly, when focusing only on the complexity of configuration, we ignore the value provided by standups. Instead, S&P focuses on value provided to standup team members. Standup reports must be timely for the team member in the location they are entered in, they must also be visible. In the case we are waiting ~24hr before viewing, there are many things in a **#channel** that might push the report out of view. This makes it impossible for the report to useful. Conversely, if we post immediately, then only one team get's the benefit for timeliness. To optimize every location's standup potential, we actually want to control exactly every location separately.

Creating a separate standup for each timezone provides additional solutions such as:
* Different timezones can see their standups exactly when they need to.
* Channels without additional conversation (i.e. a dedicated #standup-channel will have the standups grouped together anyway, since there are no other posts there, so posting times differences are negligible).
* Different teams can potentially answer different questions, so specifically: `what does team A want to convey to team B, whom will be awake in 8 hours?`.
* Users may travel between timezones, and almost all never update their slack timezone, which causes additional confusion on when they should report and who they report with.
* Different timezones usually mean different cultures and specifically holidays. Disabling a standup for a week is doable in a timezone, such complexities would not be possible in a shared standup.

#### I still want a multi-timezone solution
We are happy to work with you to design a solution that handles your team's standup value proposition. Our recommendation is to set up multiple standups one for each timezone, try it out, and let us know about anything that doesn't work. We can work together to create improvements that target those problems.

## Q: The owner of the standup is no longer part of the Slack workspace
Any member of the standup (not any member of slack) can edit a standup. If there is a standup currently reporting that you don't have access to, the best thing to do is message the channel asking to be added to the standup. If there is a need for different standup roles for different standup access (edit configuration, review reports, answer standup), upgrade the account to [Support Standard](https://standup.teaminator.io/app/?install=false#/settings?focus=standard).

## Q: What are the Standup & Prosper hidden commands?
There are two kinds of messages the bot responds to:
* `/standup` (or `/prosper`) `CMD` a list of these are available at `/standup help`
* Direct messages to the bot, a list of these is available by clicking the `Home tab` - `Help!` button or messaging the bot `I want some help`.

## Q: How to set a reminder on Friday for a Monday standup?
There is a dedicated reminder time that exists `The weekend` reminder. Create a second standup just enabled for `Monday` and set `the weekend` as your reminder time.

![image](https://user-images.githubusercontent.com/5056218/132479086-f4e017d3-0f60-443e-85a0-dcb4ec23d421.png)

## Q: Why was the standup 5 minutes late?
Unfortunately, I am not a Swiss train, I don't run exactly on time. I had a conversation with my developers, and they agreed to permit me some flexibility in scheduling of messages. Did you know there are lots of things that can get in my way, be it the network connections are down, my cloud provider is having troubles, or Slack is rejecting incoming messages. While I try to do the best I can, I do aim for the report time, **plus or minus five minutes**. I hope this works for you. If you could be a bit understanding, as I have millions of messages I need to handle every day, this helps me get them all delivered correctly. Consider me your standup Santa Claus:

🦌🦌🦌🦌🦌🦌🦌🦌🛷🤖🔔

## Q: How to stop the bot from mentioning users?
When the bot posts the report to the channel, the users of the report are tagged so they are aware that it is time to review the standup report. This functionality can be turned off `Notify users of a standup when it posts`.
![image](https://user-images.githubusercontent.com/5056218/149374584-ccaac992-f0c8-428f-bf04-4ef979e460a2.png)

