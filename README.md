# Asphalt8_Patcher
Tools to make Asphalt 8 on PC playable again!
This project is focused on older versions of Asphalt 8 (version 4 and older). The goal is to come up with a patch that circumvents cheating checks in later versions of the game while preventing it from checking for updates or retrieving ads. Essentially, make the game "offline" while still allowing some features like local multiplayer to function properly.

*Please note:* For this project, I will be primarily focusing on the Windows ports of the game which run on Windows 8 and later. I would really appreciate help for fixing older versions of the game on other platforms (Android, iOS(?), Windows Phone(?)) once I've got track on the PC fixes.

# Goals for this project
This project is going to take quite a bit of work, but since I will be working with much older versions of the game, I'm hoping it will be a bit simpler. Here are my primary goals for this project:
- Keep the game from realizing there are updates
- Disable ads
- Create a tool that allows for backing up & restoring save data for the game
- (Possibly) allow local multiplayer

The first two goals ideally require figuring out what server the game is using to check, and either blocking or reverse-engineering it (hopefully not the latter). Otherwise, on Windows, it's as simple as blocking inbound connections for the game (NOT outbound connections; the game will detect this and ban you). *Again, I would seriously appreciate any help with figuring this out since I have no prior reverse-engineering experience. I tried both Wireshark and TCPView, but couldn't narrow it down.*

# Why this project?
I remember when I first played Asphalt 8 back in 2013/2014 on my first laptop: a Gateway NE56R41u running Windows 8. I loved the game's concept, and I thought the different modes (Infection, Elimination, etc.) were really cool ideas for the 9-year-old me. Going back to play it now, and it's an ad-ridden, pay-to-play mess; not the Asphalt 8 that I remember.

I created this project because I can't imagine I'm the only one who feels like this. Having just graduated from highschool at the time of writing, I'm on a "huge nostalgia high", so I decided to try and create a patcher to make older. playable versions of Asphalt 8 work fully offline, possibly with multiplayer capability.