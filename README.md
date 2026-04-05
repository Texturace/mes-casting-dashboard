# Creator Personal Update (4/5/2026)
I'm currently pushing v1.1.0. There are a handful of QoL bugs to work through, but I want to get this update out because I'm moving halfway across the country and likely won't have another chance to troubleshoot until the very end of April (or even until May). As always, if you run into issues or have feature recommendations, please reach out to me. Until v1.1.X gets released to address bugfixes, if anything is flat-out breaking, then just roll it back to the previous version.

# MES Casting Dashboard
This is a companion app to Streamlabs/OBS to allow for higher quality content when casting. It provides a Draft Screen, Head-to-Head Screen, Brackets, and Groups. As this grows, I will attempt to incorporate Riot API and Drafter API to improve quality of life, and to eventually create in-game templates as well. Currently, everything relies on manual inputs in the dashboard. v1.0.6 is the first official release (previous versions were internal testing or included updates suggested by people interested in the project).

Current release download: https://github.com/Texturace/mes-casting-dashboard/releases/tag/v1.0.6

Video demonstration of me using the tool: https://youtu.be/b9MbJszumbY

## Current Features
- Fully functional draft (Picks and Bans populate in the correct order AND each lock-in has a spotlight animation)
- Role Assignment Menu (Assign picks to roles so that other screens appear correct)
- Head-to-Head screen (Upon swapping to H2H, a spotlight animation happens by role with player names)
- Full team creation (Upload logos, enter player names, assign player roles)
- Bracket Creation (Create Single and Double Elimination Brackets)
- Group Creation (If you're not in play-offs, then this is a way to keep track of matches as they progress throughout the season. Convenient screen to update viewers on the status of the league)
- Tournament Selection (Add teams under tournaments so that you don't end up with a list of 40 teams. Each tournament saves the correct subset of teams, and it should save bracket/group information as well)

## Hopeful Future Updates
- Riot API Implementation: Part 1, pulling Solo Queue stats (e.g., BlueJungler {Xin Zhao} 4-3 (57.14% WR) {KDA}); Part 2, creating custom in-game overlays that always track gold/stacks/etc.
- Drafter API Implementation: Why manually input everything in the draft menu if we can just pull everything (along with the timer) from Drafter itself?
- Cross-Platform Functionality: 95%+ of you are probably running everything on Windows, but enabling MacOS support (and Linux support for those casting from Linux while using a capture card from a computer running Windows/MacOS ... AKA me in June/July 2026)
- ~~Multiple Resolutions: Currently, everything only works for 1920x1080, but it's possible that I can build some type of toggle that would allow you to broadcast from the "standard" resolutions of HD, QHD, and UHD.~~ (v1.1.0)

## What to do if Things Break
1) Click "Send to Overlay": I have found some non-replicable bugs here and there that have all been resolved by clicking the "Send to Overlay" button. If you find a bug that IS replicable, please send me detailed steps and screenshots for me to troubleshoot and correct the issue.
2) Refresh Streamlabs Sources: Throughout my testing, if I encounter an issue that doesn't get fixed by "Send to Overlay", then it gets fixed by refreshing the source. These are all HTML files, so "Source Name" -> "Refresh cache of current page" (Streamlabs). I will be switching to Linux in the near future and will update with vanilla OBS instructions later (though I assume it's nearly identical, if not identical).
3) If you are having issues UPDATING the Dashboard, then check your equivalent of Task Manager and force end processes (MES-Casting-Dashboard with the "all lanes" icon). Closing the application *should* "shutdown" the local server you created by running the application, but if there are errors when installing, then it can get stuck.
4) Reach out to me: If there's genuinely an experience-ruining bug, I will do what I can to remediate the situation. I will try to troubleshoot the issue and push an update as quickly as possible (though, depending on my work schedule, that might take upwards of a few days). If there are substantial issues, then I can also extend licenses to make up for downtime/issues.


### Acknowledgement
This project was originally developed as an in-house tool for Maelstrom eSports. If you want more information about the organization, there is a "Shameless Plug" at the bottom of the README. 
This project was motivated by EsportsDash (https://docs.esportsdash.com). EsportsDash is a great, open-source project that works for a variety of games. Currently, it doesn't have the functionality that I wanted/needed for my use case, so I built my own application. That is not a knock against their dashboard or their team. The dashboard is great. I have experimented with it. They have a lot more flexibility with their dashboard, but that flexibility comes at the cost of depth. I had to personally add new champions on my local machine, the basic template is designed around games that have a variety of maps (bring back Twisted Treeline </3), and there's no native API implementation/support (as far as I could tell, but I could be wrong).


### Licensing
This project did take a substantial amount of time to troubleshoot and create. I'm not certain about Riot API, but I know that Drafter API access requires a monthly subscription ($20 + you have to create all the draft links *through* the API). The goal of licensing is never going to be to make a substantial amount of money.
- Licensing will cover my external licensing fees as more implementation is developed.
- Licensing will help me afford 2-ply toilet paper instead of 1-ply.
- Licensing will go back into MES to help pay coaches and fund team entry fees.
- An eventual domain so that I don't have to use a generic "onboarding@resend.dev" email for key distribution
  
If you need anything special, please email me at "mes-dashboard.claim881@passmail.net". As the sole admin, I have the power to create custom keys. If you need a special arrangement, then we can work something out.

For general needs, you can select which plan fits best here: https://texturace.github.io/mes-casting-dashboard/

## Shameless Plug
### Maelstrom Esports Player Association (MESPA)  applications ARE NOW OPEN!

🔥
 What We’re Building:

Maelstrom Esports is searching for dedicated players and coaches of all skill levels to join MESPA. MESPA is focused solely on helping players improve, rank up, and achieve their desired level of competition. MESPA is not looking for the best players or championship-winning rosters. We want players who are struggling, hardstuck, or just don’t know how to push through the next rank.

MESPA Players will be placed in a team with like-minded individuals and dedicated coaches, all focused on improvement and ranking up.  Our 5 most dedicated and best preforming players in a skill group will be offered invitation to an "Allstar" Team.  "Allstar" Teams receive paid tournament entry from MESPA- For other MESPA teams who want to compete, entry fees must be covered out of pocket. 

Promotion to the next skill group is earned through SoloQ rank progression, team play improvements, and consistency. If you put in the work, you can climb all the way to the NACL team. FREE individual coaching is also available through our ticket bot to help you reach your goals

MESPA Coaches will be assigned a team to help them improve and advance to the next division. They primarily focus on teamplay, though may offer individual coaching. Coaches gain valuable coaching experience, and are subject to promotion

Community Members have access to all of our resources, including the FREE  1-on-1 coaching we provide at Maelstrom. You do not need to be a member of any of our teams to be a part of the community. All you need is to join the Discord and select the MESPA Role.

For those who have peaked 700+ and want to make the push into
🔑
 How to Apply:

Head to our application sheet:

MESPA Players (Iron-1k): https://forms.gle/q3LqXqAvP5CgQMyf7 

MESPA Coaches: https://docs.google.com/forms/d/e/1FAIpQLSfuT6x9xzRcZ57UNlGbVxiyz0vjkHS_gNUH36l2bTRMb_dl7w/viewform

MES Uncapped/OQ (Players & Coaches): https://forms.gle/DuAs5yKk2qqVHFSBA

Fill out the form
Submit your application
Wait for us to contact you via Discord (make sure DMs are open and you entered your username correctly)
