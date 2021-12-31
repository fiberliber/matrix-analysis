# Matrix element.io proc and cons report

In addition to my own analysis of element code, I'm also makes a research of sosial and technical resources for meaning about comparison of element.io (riot.im) with other group chat platforms

There a list of resources, which have a ready to use compare charts:
[Sourceforge](https://sourceforge.net/software/compare/Discord-vs-Element-Messenger-vs-Mattermost-vs-Slack/), 
[Stackshare](https://stackshare.io/stackups/discord-vs-mattermost-vs-riot-im0), 
[Slashdot](https://slashdot.org/software/comparison/Discord-vs-Element-Messenger-vs-Mattermost-vs-Slack/), 
[Slant](https://www.slant.co/topics/10806/versus/~mattermost_vs_slack_vs_discord)

Also can be easy founded interesting posts of that theme on [Medium](https://medium.com/ignation/time-to-replace-slack-who-will-win-mattermost-or-riot-matrix-a090e9cdc219), [Reddit](https://www.reddit.com/r/selfhosted/comments/7k471o/zulip_vs_rocketchat_vs_mattermost_vs_riotim_slack/), [Opensource](https://opensource.com/alternatives/slack) 

In the internet present a lot of publications with very different means and opinions, but from all properties of any platform, we can select a main features, which related to any platform and play as key characteristics

<hr/>

### Privacy and safety capabilities

Most platforms use SSL/TLS for data protection and do not use E2EE principles for that. 

However, centralised security allow that organization leverage user access to data and services, because all interactions should be signed by centralized controlled CA.
Other cons of that type of security, is compromized user local trusted CA database and in generaly necessary to trust that authority centers in cases if some from that will be compromized itself.

`element security proc:`

In this sense, element have a great advantage over such platforms, because provide to the users a way for establish secured channels, independent from central authority, but this nuanse is a medal with two sides: central authoryty needed for ultimative MITM prevention and currently is once known way for [two generals problem](https://en.wikipedia.org/wiki/Two_Generals%27_Problem) solution.

`element security cons:`

Device verification, used in element, is a partialy method for prevent very pure permanent MITM attack, and using double ratched keys derivation is good principle for prevent MITM intrusion in middle of data exchange process, but all that tools unefficient versus permanent AI powered MITM, which able to deep analyse intercepted traffic on a fly, include media data recognition, machine learning and complex media generation (deep fake algorithms).

`how element security can be improved:`

For improve element security I strongly recommend to distribute clients with predefined CA signatures and add public keys and shared keys signing for additionally ensure end-to-end trust. Also, for future security versus quantum computation powered MITM, allready have a sense to change shared secret exchange algorithm from ECDH to [SIDH](https://en.wikipedia.org/wiki/Supersingular_isogeny_key_exchange) 

<!--
`what R&D can be initiated for enhance element cryptography:`

I have made some research in newest cryptography direction, called "interpretative cryptography", which look on a key not as on passive data, used for mixing with clear text for encryption, or signing, but as unique random algorythm as is. In the base of idea a fact, that we can interpriate any arbitrary sequence of bytes as some algorythm by endless count of interpretation methods (IM's). This is mean, that we can sync, using SIDH keys exchange IM on remote sides, and then even derive for some encrypted data other IM, which can adopt encrypted data for direct reencryption in a form, encrypted by other key, whithout needs to decrypt it in open form. This is very early experimental technology, which should be deep researched a lot, but that have a potential to make a revolution in a cryptography globally. For example, In a current standards, every E2EE channel use a some wellknown block cypher algorythm for every keys pair, but in concept of interpretative cryptography, for each keys pair will be generated unique block cypher algorithm, defined only by sequence of bytes in a concreat shared secret and works using an unique fresh festel network realization, unlike anything known, like AES, chacha20, polypoly and so on. Nice property of that technique is this block cypher works as a streaming encryption, which can encrypt or decrypt data on a fly and stay a quantum resisted. Main R&D in that cryptography type is found asymmetric interpretative keys exchange (as a replacement of SIDH), which can be multitenant (support any quantity of encrypted data exchange participants) without exponential grows of same data encryption forms and without needs of common for group shared key transfers (in combination of [dinner cryptographers principle](https://en.wikipedia.org/wiki/Dining_cryptographers_problem))
-->
<hr/>

### Opensource/proprietary code and cross-platfom support

Main difference between opensource and proprietary code license is in dev team responsibility and contribution style in a project development. Often proprietary code teams have more responsibility, in comparison to opensource, because all support and integration processes often are paid, or depend on dev team access to the clients data. Closed code have only one advantage over open - keeping a know-how's in a secret, which can give to the company technical advantages only if that technology really have no alternatives. 

In most cases, making a code open, and lisensin it as free software, allow teams lagging behind the technical leader, teams lagging behind the technical leader, quickly attract a community of enthusiasts to the development, if the project is interesting enough in itself, and if it is also [monetized](https://thenewstack.io/options-for-monetizing-your-open-source-project/), or when using the project code in many other projects (libraries, modules, scripts, etc.), additional motivation appears, helping not only to attract many interested humans, but also to get high-level professionals into contributors.

Another difference, that in propietary model, cross-platform project expansion supplyed by employees of some company, which depend on grow often hight paided staff count, but in opensource model, expansion can be maded and by core team, and by some other developers, or even companies, which interested in additional platforms support.

`element model proc:`

It is opensource and available for absolutely free usage - that allows element grows quickly and cover many platforms, thanks to the work of many independent teams, at the same time, the [monetization model](https://element.io/matrix-services/ems-pricing) allows them to create additional motivation for project participants

`element model cons:` 

No cons - all cool

<hr/>

### Integrations and architecture

Architecture of any droup chat platforms, usually assumes the presence of such functional as privat chats, group chats, ability to create dedicated multirooms space for come project, or orfanization, or just a people group with common interests and accorfing to that interests propose variouse integrations with third side online services for different purpose, like a games, project management, collaboration tools, internationalization, financial instruments and so on. This is obliges a platforms to have a very complex architecture, with back end, powered by different databases with flexible unordinal data scheme, supporting a lot of side API's and very flexible extansible front end.

`element model proc:`

Main element architecture preferrencies is distributed synapse nodes network behind the scene, which makes whole ecosystem very resilent and diversified, Also a services specialization principle, in a base of division on main nodes, identify services and bridges, make system more simple and provide easy support and system enhancement. Opensource integrations API open a ways for riachment additional functionality ecosystem, but...

`element model cons:` 

Element integrations don't use integration managers and API aggregators, relying only on matrix developed code and this is limit interoperability with third side solutions.

`how element integrations can be improved:`

In addition to own realisation of side services API, good idea will be integrate with [API aggregators](https://www.tecmint.com/open-source-api-gateways-and-management-tools/), which already containse ready to use implementations of high count of variouse services and provide unified API to interact with they are

<hr/>

### Target audience and limitations



<!-- users, group chats and virtual servers (rooms, organizations, etc) -->
<hr/>

### Usability (UI/UX), support and Documentation


