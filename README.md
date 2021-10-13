# The Standup and Prosper FAQ
Below are listed some common answer for a little more complex activites in S&P

## Q: I can't find an answer to my question
Click [Create a new issue](https://github.com/Teaminator/Standup-and-Prosper-FAQ/issues/new) and ask away, or if you figured out something that you want everyone to know, just click [edit the FAQ](https://github.com/Teaminator/Standup-and-Prosper-FAQ/edit/main/README.md). (You'll need an account for this). If neither of those are options that work for you, send an email to the [Standup Support DL](mailto:faq-support@teaminator.io).


## Q: How to make standups aware of the user's timezone?
A common question about scheduling is "I want to have every user in the standup get reminded at 10:00AM in their timezone to answer the standup, how do I do this?". Great, the best way to achieve this for your team is to create one standup in each of the timezones where the users are, and assign just the users to that standup. It might seem that it would be better to have a single standup, which has a single report time, however that's actually not the best pattern. Let's take a look at some common problems that the multi-standup approach solves. For this, we'll assume there is one team in EST (UTC-4) and one team in IST (UTC+5.5):
* If the report time is at 5PM EST--then IST enters their standup at 10AM IST, but the report happens at 2:30AM IST that's not valuable for that team that has to wait 24 hours until they are in the office the next day to see the standup of their own team members. Likewise, the team in EST, also is waiting until the next day.
* If the report time is at 12PM EST--then IST enters their standup at 10AM IST, but the report happens at 9:30PM IST. That fixes the problem for EST but not IST.

Commonly, when focusing only on the complexity of configuration, we ignore the value provided by standups. Instead S&P focuses on value provided to standup team members. Standup reports must be timely for the team member in the location they are entered in, they must also be visible. In the case we are waiting ~24hr before viewing, there are many things in a **#channel** that might push the report out of view. This makes it impossible for the report to useful. Conversely, if we post immediately, then only one team get's the benefit for timeliness. To optimize every location's standup potential, we actually want to control exactly every location separately.

Creating a separate standup for each timezone provides additional solutions such as:
* Different timezones can see their standups exactly when they need to
* Channels without additional conversation (i.e. a dedicated #standup-channel will have the standups grouped together anyway, since there are no other posts there, so posting times differences are negligible)
* Differnt teams can potentially answer different questions, so specifically: `what does team A want to convey to team B, whom will be awake in 8 hours?`
* Users may travel between timezones, and almost all never update their slack timezone, which causes additional confusion on when they should report and who they report with.
* Different timezones usually mean different cultures and specifically holidays. Disabling a standup for a week is doable in a timezone, such complexities would not be possible in a shared shared.

#### I still want a multi-timezone solution
We are happy to work with you to design a solution that handles your team's standup value proposition. Our recommendation is to set up mulitple standups one for each timezone, try it out, and let us know about anything that doesn't work. We can, together to create improvements that target those problems.

## Q: What the Standup & Prosper hidden commands?
There are two kinds of messages the bot responds to:
* `/standup` (or `/prosper`) `CMD` a list of these are available at `/standup help`
* Direct messages to the bot, a list of these is available by clicking the `Home tab` - `Help!` button or messaging the bot `I want some help`.

## Q: How to set a reminder on Friday for a Monday standup?
There is a dedicated reminder time that exists `The weekend` reminder. Create a second standup just enabled for `Monday` and set `the weekend` as your reminder time.

![image](https://user-images.githubusercontent.com/5056218/132479086-f4e017d3-0f60-443e-85a0-dcb4ec23d421.png)


