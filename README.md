# Windows Safe Browsing Chrome Policy. Simple to deploy.
Deploy these Google Chrome policies via Registry tweaks on your Windows machine to maintain a safe internet environment for you and your family and/or kids.

The benefit here is that these policies are enforced on your machine within the OS itself, as opposed to trying to filter content on the networking side (which can be effective but is much more difficult to keep airtight as workarounds are constantly available).

NOTE: Always export a backup of your registry keys and settings before making any changes.

Import these registry changes to create a safe and virtually inpenetrable internet environment for those who choose to stay away from inappropriate adult content and other distractions. Registry settings are updated in the following hive -> "[HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome]". Local machine ensures the settings apply to any user on the device itself.

Features include:
- Force Google Safe Search
- Force Youtube Restrictions (Google conveniently provides levels of restriction for flexibility)
- Google Image Search Blocked
- Disable Incognito Mode
- Only allow specific websites (upto 1000 can be provided)

How to Deploy:
- clone/download .reg and .bat files
- open command prompt with Admin privileges and CD to the directory where the 2 files are located
- run "deploy.bat" and restart your browser for new settings to take effect

Notes:
- It is imperative that the user(s) do not have Admin privileges which would allow these registry settings to be adjusted.
- It is also recommended that the user is unable to have access to any other browser or installing msi files or downloading from MS app store
- Microsoft Family actually does a decent job in app limits and other restrictions, but is not very robust when it comes to actual internet browsing.

See https://github.com/ahprh12/Bailey-Cloud-DNS-Proxy-Filter for a POC solution provided from the networking end. I've found that is an ongoing challenge to keep up with all the loopholes and means that allow users to bypass even the most complex internet filters. Popular content filterings solutions such as Covenant Eyes or Pi-Hole backed by Steven Black Unified Hosts (https://github.com/StevenBlack/hosts) have done an incredible job in creating a safe environment for humans everywhere, but there are always ways to break the system. The solution here is to only allow specific web sites and block everything else, which is a very aggressive tactic for internet safety, but one which I find invaluable. Yes, tons of false positives are blocked, but it is worth it for me. Questions and feedback are always welcomed.
