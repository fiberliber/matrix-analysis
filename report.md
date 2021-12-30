# Matrix element.io proc and cons report

In addition to my own analysis of element code, I'm also makes a research of sosial and technical resources for meaning about comparison of element.io (riot.im) with other group chat platforms

There a list of resources, which have a ready to use compare charts:
[Sourceforge](https://sourceforge.net/software/compare/Discord-vs-Element-Messenger-vs-Mattermost-vs-Slack/), 
[Stackshare](https://stackshare.io/stackups/discord-vs-mattermost-vs-riot-im0), 
[Slashdot](https://slashdot.org/software/comparison/Discord-vs-Element-Messenger-vs-Mattermost-vs-Slack/), 
[Slant](https://www.slant.co/topics/10806/versus/~mattermost_vs_slack_vs_discord)

Also can be easy founded interesting posts of that theme on [Medium](https://medium.com/ignation/time-to-replace-slack-who-will-win-mattermost-or-riot-matrix-a090e9cdc219), [Reddit](https://www.reddit.com/r/selfhosted/comments/7k471o/zulip_vs_rocketchat_vs_mattermost_vs_riotim_slack/), [Opensource](https://opensource.com/alternatives/slack) 

In the internet present a lot of publications with very different means and opinions, but from all properties of any platform, we can select a main features, which related to any platform and play as key characteristics

### Privacy and safety capabilities

Most platforms use SSL/TLS for data protection and do not use E2EE principles for that. 

However, centralised security allow that organization leverage user access to data and services, because all interactions should be signed by centralized controlled CA.
Other cons of that type of security, is compromized user local trusted CA database and in generaly necessary to trust that authority centers in cases if some from that will be compromized itself.

In this sense, element have a great advantage over such platforms, because provide to the users a way for establish secured channels, independent from central authority, but this nuanse is a medal with two sides: central authoryty need for ultimative MITM prevention and currently is once known way for [two generals problem](https://en.wikipedia.org/wiki/Two_Generals%27_Problem) solution.

Device verification, used in element, is a partialy method for prevent very pure permanent MITM attack, and using double ratched keys derivation is good principle for prevent MITM intrusion, in middle of data exchange process, but all that tools unefficient versus permanent AI powered MITM, which able to deep analyse intercepted traffic on a fly, include media data recognition, machine learning and complex media generation (deep fake algorithms).

For improve element security I strongly recommend to distribute clients with predefined CA signatures and add publick keys an shared keys signing for additionally ensure end-to-end trust. Also, for future security versus quantum computation powered MITM, allready have a sense to change shared secret exchange algorithm from ECDH to SIDH 

### Opensource/proprietary code and cross-platfom support
### Integrations and architecture
### Target audience and limitations
<!-- users, group chats and virtual servers (rooms, organizations, etc) -->
### Usability (UI/UX), support and Documentation


