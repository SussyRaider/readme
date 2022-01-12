# 〜HOW TO USE SussyRaider〜

### [Here](https://hackmd.io/@hIcQaeazRBmc_QUFj5HjlQ/BJz0vOuiF) is a version that is easy to view

[:warning:] It is currently in Beta, so the only modules available are Join/Leaver and Spammer  
  If you want to use the existing features, use the old version!
  
![](https://cdn.upload.systems/uploads/DAZQJDDk.png)


- This guide is for the idiots who can't figure out how to use SussyRaider lol
- This guide was last modified on [2022/1/12 4:42 PM JST].
- BruhTea#4000

## Prerequisite
- SussyRaider has been tested and supported only on **Windows 10, 64bit** environment
    - It may not work properly on other versions of Windows (**only a possibility**)
    - Operation is not guaranteed in any environment other than Windows 10, 64bit environment
- Fast internet connection (50Mbps up and down is good)
- Smart brain
- The ability to solve problems on your own, even if you encounter them

## Requirements
- A PC with sufficient performance with Windows 10 64bit
- Discord Token
- High quality proxies

## Create Account & Log in
SussyRaider requires you to create an account to use it (first time only)  
1. first create a ticket from `#hwid-issue` on the [official server](https://discord.gg/Cdee9PTRg8) and punch the Devs to get a license key
2. once you have the license key, go to [SussyRaider's registration page](https://sussyraider.cc/register) and register an account.  
   Put your license key in the last place!  
   ! [register sample](https://i.imgur.com/sK7Kfad.png)
3. close the ticket you went to punch in once you've registered, because Devs get tired
4. launch SussyRaider, enter your username in the `userid` field and your password in the `password` field, then press `LaunchSussy`
5. SussyRaider will start bruh

## Operate Module

### Proxy and Token settings
Basically, SussyRaider loads the proxy first, then the token  
As shown in the screenshot, select the type of proxy you want to use, check `Use Proxy`, check the proxy, and finally load the token.

![](https://cdn.upload.systems/uploads/Afq8D4Af.png)

You can set the delay by using Set Delay
- [ℹ️] Delay 1 = 1 second

This will be applied by pressing Apply

![](https://cdn.upload.systems/uploads/bScI5V2R.png)

[:x:] **Check the Use Proxy checkbox before loading the token  
In the worst case, your IP will be restricted by Discord**
- If you have a small number of tokens (1~5) you (maybe) able to use without it

### Join/Leave
If you want selfbots to enter the server, put the invite link to `InviteLink`  
After entering the invitation, press `SelectALL` on the left tab or select the token you want to use  
After selecting the token, press `Join` to let the bot enter the server  

To bypass member screening, check the `Bypass Member Screen` checkbox and enter the server ID before entering the room  
To leave the Token, enter the server ID in the `ServerID` field  
Press `Leave` to exit the bot from the server

![](https://cdn.upload.systems/uploads/rb9p0Qov.png)

### Server Spammer
Put the ID of the server to be spammed in `ServerID` and the ID of the channel to be spammed in `ChannelID`

#### Button description
┣ All Ping : Send a ping to all members in the server. (If the server has 1000+ members, only online members will be pinged)  
┣ Spam to All Channel : Spam to all channels on the server where you can speak  
┣ Random String : Inserts a random string at the end of the text to be spammed  
┣ RateLimitFixer : When a rate limited, this will pause sending requests until the rate limit is end  
┃  
┣ Mention : Sets the number of people to mention in All Ping, only works when All Ping is enabled  
SpamMessage : Enter the text to be spam here

You when have to spam, enter a message in the Put the message in the `Content` field and press `Add Content` to add the content (you can add more than one of these)  
Start spamming with `Spam Start`, and if All Ping is enabled, fetch the members and then start spamming.  
Press`EndSpam` to stop spam

[:warning:] All Ping is unstable and may not work. If you stop it and then start it again, it may work

### Report Spam
You can report spam on the Discord API. Please note that this is not a report from [here](https://support.discord.com/hc/en-us/requests/new)  
Please put the server ID in `ServerID`, the channel ID in `ChannelID`, and the message ID in `MessageID`
#### Report Type (Reason for the report)
┣ Illegal Content (Illegal content, including 2D loli images, etc.)  
┣ Harrasment (Harassment, etc.)  
┣ Spam or Phishing Links (links to spam or phishing sites, etc.)  
┣ Self harm (suicidal behavior etc.)  
┣ NSFW Content (pornographic content on non-NSFW channels, etc.)

You can start a report by clicking on `ReportSpam` at the top.

### Nickname/Avatar change (Nick/Avator)
Instantly change your bot's nickname or avatar

- To change your avatar, enter the image link in the `Avator URL` and click `ChangeAvator`.
- To change your nickname, enter your server ID in the `ServerID` field, enter your nickname in the `Nickname` field, and click `ChangeNick`

[:information_source:] Originally, the spelling of "アバター" should be "Avatar". However, the creator of this one thought what he was doing and wrote "Avator". This is either a joke or a sign that the creator is weak in English lol

### Friend/DM spammer
You can spam friend requests or DMs

- If you want to spam a friend request, enter the name in the form of a tag in the `User` field and click on `FriendSend`.

- To spam DMs, enter your user ID in the `UserID` field, enter the message you want to spam in the `SpamMessage` field, and click `DMSpammer`

[:warning:] DM spam should not be used too often, as it tends to reduce the life of Tokens

### Voice Spammer
Allows you to spam voice channels.

[:heavy_check_mark:] Before using the VC spammer, make sure you have `ffmpeg.exe` and `libopus.dll` in the same folder as the SussyRaider exe file.


1. Add the VC ID to `Voice Channel ID` and the server ID to `ServerID`
2. Select `VoiceFile mp3` and select a music file in .mp3 format
3. Click on `VoiceSpammer` to spam the VC

### Reaction Spammer
This is broken because the productor is lazy Therefore I cannot write it lol

### Button Pusher
This function allows you to push buttons such as Ticket Bot.

Enter the server ID in the `Server ID` field, the channel ID in the `Channel ID` field, the message ID in the `Message ID` field, and press Send

[:warning:] This module may be unstable

## You SHOULDN'T do it
- Use WITHOUT proxies (okay if you only use a very small number of selfbots)
- Sending DMs and friends around
- Spamming for a very long time
- Voice spamming with 100 tokens or more
- Use voice spam many time

## FAQ
- Q. What is a proxy?  
 ┗ A. It is a relay server to prevent your IP from being restricted. Most free proxies are garbage, so you should buy one. I recommend [Proxyscrape](https://proxyscrape.com) Premium.

- Q. What is Token?  
 ┗ A. Ask someone else for the details, it's hard to write

- Q. I enabled All Ping and started spamming, but it doesn't say anything all the time? Is it a garbage tool? Hey?
 ┗ A. If it looks like you are not getting members, etc., try stopping and then starting again. (If you are able to get members, `[+] Get <USERID>` will appear in the console.)

- Q. Why can't I use Onliner or Reaction?  
 ┗ A. As for Onliner, it's not implemented yet, and Reaction says it's broken meh

- Q. Why can't I see what I've said when I start spamming?  
 ┗ A. Make sure that the selfbot is not muted or kicked. Also, please check your server's authentication level, as it may be trapped

- Q. I don't seem to have been sent any DMs/friend?  
 ┗ A. There is a high possibility that the other person has rejected your DM/friend

- Q. I let someone in, but they left on their own?  
 ┗ A. It is very likely that Vortex or other anti-raid worked. Please set the delay and try again

- Q. Why can't I leave the room?  
 ┗ A. Your proxy or Token may have died

- Q. I get a KeyError when I try to spam.  
 ┗ A. There is a high possibility that the bot is being kicked, banned, or not allowed to enter in the first place

- Q. I got a "Rate Limit!  
 ┗ A. Discord has a rate limit on it. In most cases, this will be removed in a few seconds, so don't worry too much about it

- Q. What is member screening?  
 ┗ A. This
![](https://pbs.twimg.com/media/EpyO3E6VQAA3H9Q.jpg)

- Q. I can't do any mentions.  
 ┗ A. You can't do it by doing @Nigger#1234 or something like that  
    - User Mentions: `<@userid>`.
    - Role Mentions: `<@&roleid>`.
    - Channel: `<#channelid>`.

- Q. I'm getting a 404 error and can't spam.  
 ┗ A. I think you have the wrong server ID or channel ID, please check.
 
 
If you have any other questions, please feel free to ask them in Discord!
I'm sure someone will answer (maybe)

Thanks for reading!
