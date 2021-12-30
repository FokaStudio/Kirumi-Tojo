# FAQ

<hr>

## I turned on talking functions and I can't turn them off! What do I do!

Just run `!!talk` once again and all should be fine.

Or `!!ai`, they are both the same command.

<hr>

## The percentages on the similarity between the commands are nowhere near!

Yes, I am aware that running command like `!!fdsfeisjfjdsfds` will return.

![*❓ That command doesn't exist! Did you mean !!serv - 54%?*](assets/faq/similarity.png)

For the people who are **really** interested in how this works, I suggest paying a visit [here](https://en.wikipedia.org/wiki/Jaro%E2%80%93Winkler_distance) - to see how this is actually calculated, and [here](https://github.com/FokaStudio/Kirumi-Tojo/blob/main/code/18_Similarity.sk), to see the function's origin in code.

<hr>

## The bot requests 'Mute Members' permissions in a Voice Channel! Why?

I pushed an update at some point where the Bot **requires these permissions** to be able to play music in Voice Channels.

This was done because Tojo ==was initialy muted in AFK channels and she couldn't unmute herself==.

???warning "This is a temporar change!"
	Kirumi will soon distinguish between AFK channels and regular ones, so the permissions are required only there.

!!!question "How to fix this?"
	You can do 2 things:
	???example "Re-adding Kirumi"
		!!!warning
			There is no need to remove Kirumi from the server!

			This tutorial shows you how to refresh the permissions for the bot!
	
		- **Step 1: Head over to the Members List**

			![Member's List](assets/faq/setup-1-1.png)
	
		- **Step 2: Locate Kirumi and click onto her to go to their profile**

			![Kirumi's Profile](assets/faq/setup-1-2.png)
		
		- **Step 3: Click the big `Add to server` button and re-add her to your server**

			![OAUTH](assets/faq/setup-1-3.png)

			!!!info ""
				This causes no data loss, it just refreshes permissions!

				So don't worry, there is no need to reconfigure everything :grin:
	
	???example "Editing permissions manually"
		- **Step 1: Head over to the Roles List**

			![Member's List](assets/faq/setup-2-1.png)
	
		- **Step 2: Locate Kirumi's Role and click on it to edit it**

			![Kirumi's Profile](assets/faq/setup-2-2.png)
		
		- **Step 3: Allow permission `Mute Members` to Tojo-san**

			![OAUTH](assets/faq/setup-2-3.png)

			!!!danger "Beware the non-epic fail!"
				This can sometimes fail to work if your channels don't inherit role permissions! *(e.g. `Role A` can talk in **#general**, but not in **#general-no-a**)*

				If that is the case, you have to configure those permissions in the channel's configuration as well.
