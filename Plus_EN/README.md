## Loon Tutorial

- Loon's Plus tutorial is stored in this folder.

- Please read the following **Disclaimer** carefully, any reader who clicks on the document in the tutorial will be deemed to have accepted this disclaimer.

- **When users read this document for operation, please switch the language in Loon to Chinese.**

---

### Loon official

- [LoonManual](https://github.com/Loon0x00/LoonManual/blob/master/README.md)

- [Telegram: Loon0x00](https://t.me/Loon0x00)

- [Twitter: Loon0x00](https://twitter.com/loon0x00)

- [App Store download address](https://itunes.apple.com/us/app/loon/id1373567447)

---

### Disclaimer

- This tutorial is only for users who have purchased genuine Loon to learn how to use this software. I have never provided airport services or instigated mainland users to establish and use non-statutory channels for international networking without authorization.

- Through this tutorial, users use Loon to use illegal channels for international networking and conduct behaviors that violate the laws and regulations of mainland China and its regions. I am not responsible for the consequences of such users.

- This tutorial only teaches how to configure script functions, and will never provide any specific scripts that harm the legitimate interests of natural persons, legal persons, and unincorporated organizations, such as cracking scripts.

- Please do not use the script for any commercial or illegal purposes. I am not responsible for any consequences caused by such actions.

- Anyone who reads this tutorial in any way, directly or indirectly operates the steps in this tutorial, should read this statement carefully.

- I have the right to modify and supplement this disclaimer. Any reader who clicks on the document in the tutorial will be deemed to have accepted this disclaimer.

---

### Configuration column

The purpose is to improve the user's ability to customize the Loon configuration, and write tutorials in the order of the `configuration` column panel

#### Node

- [Single node](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Proxy_EN.md) (add proxy node manually)

- [Subscription Node](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Proxy_EN.md) (subscribe to a collection of nodes, usually provided by the airport the user purchased)

- Screening subscription nodes (screening subscription nodes into proxy nodes that users need, reducing too many proxy nodes to appear in the policy group, and making it easy for users to choose the proxy nodes they need)

  - [Regular expression](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Regex_EN.md) (Master the basic regular expression writing)

  - [Filter method with filter type `NodeSelect`](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Filter_NodeSelect_EN.md) (manually filter nodes)
  
  - [Filtering method with the filter type `NameKeyword`](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Filter_NameKeyword_EN.md) (Use keywords to filter subscription nodes, but nodes cannot be excluded)

  - [Filter method with filter type `NameRegex`](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Filter_EN.md) (Use regular expression to filter subscription nodes)

- Use Sub-Store to filter subscription nodes (simple, efficient and convenient) (There is no English translation in this tutorial)

  - [Text Tutorial](https://www.notion.so/Sub-Store-6259586994d34c11a4ced5c406264b46) (There is no English translation in this tutorial)

  - [Video Tutorial](https://www.youtube.com/watch?v=VXlQ4kDgqSE&t=171s) (There is no English translation in this tutorial)

- [Nesting between node and policy group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Proxy_in_Proxy_Group_EN.md) (add proxy node under the policy group)

#### Strategy

- Loon without default proxy policy group

  - [Proxy Policy Group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Default_Proxy_EN.md) (Understand the proxy policy group, with [understanding of global policy](https:// github.com/chiupam/tutorial/blob/master/Loon/Plus_EN/Global_Group.md) tutorial)

  - [Understanding of the global strategy](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Global_Group_EN.md) (the reason why the global agent must be used with the global strategy)
  
- [New Policy Group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/New_Proxy_Group_EN.md) (manually add a sub-policy group)

- Parent strategy group and child strategy group

  - [Correctly distinguish between parent policy group and child policy group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/TOP_Policy_EN.md)

  - [Russian dolls-nesting between child and mother strategy groups](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Matryoshka_EN.md)

- Three commonly used automatic strategy groups

  - [Set URL-Test Policy Group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/URL-Test_EN.md) (preferably the lowest latency)
  
  - [Set Fallback Policy Group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Fallback_EN.md) (health check)
  
  - [Set PCC policy group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/PCC_EN.md) (the same host name locks the same node)
  
- Set SSID policy group

  - [Method 1: Setting of built-in ssid strategy group](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/ssid_EN.md) (This tutorial needs to understand more concepts and is relatively simple, Not flexible enough)
  
  - [Advanced Operation: Nesting of ssid Strategy Groups](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/ssid_Plus_EN.md) (The operation is extremely cumbersome, but it is difficult to meet the requirements Understand, novices, users who are impatient, please detour) (unfinished)

  - [Method 2: Script method](https://t.me/cool_scripts/141) (SSID script is recommended, thanks to Peng-YM, please do not chat privately!)

#### Rules

- [What is a rule](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Rule_Summary_EN.md) (the reason for the design rule in the agent software)

- [Single Rule](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Rule_EN.md) (Add a local rule manually through the UI)

- [Subscription Rules](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Rule_EN.md) (Subscribe to a collection of rules and select the parent policy group)

- [Recommendation Rules](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Rule_Recommend_EN.md) (recommend common rules for novices)

- [Final Rules](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Final_EN.md) (the rules of the rules)
 
#### Plugins

- [Preliminary understanding of plug-in functions](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Plugin_Summary_EN.md) (Powerful custom configuration artifact)

- [Add URL requirements and content format requirements in the plug-in](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Plugin_Format_EN.md) (a must-see for newbies)

- [Add a plugin](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Plugin_EN.md) (add a plugin)

- [Recommended plug-in URL](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Plugin_Recommend_EN.md) (organize more practical plug-ins for novices)

#### Rewrite

- [Rewrite](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Rewrite_EN.md)

#### Scripts

- [Learning basic cron expressions](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/cron_EN.md) (modify the execution time of the timing script)

- Use scripts in Loon (from getting started to giving up)

  - [Getting Started-How to understand the necessary format of the three script statements](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/JaveScript_Format_EN.md) (a must-see for novices)

  - [Elementary-How to understand a script configuration code](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/JaveScript_1_EN.md) (Resolve the confusion of configuration scripts)

  - [Intermediate-How to write script configuration code into Loon to play a role](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/JaveScript_2_EN.md) (required for script execution)
  
  - [Advanced-API Document Reference](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/JaveScript_3_EN.md) (high-level players)
  
  - Abandon —— Script execution still fails (Sorry, I do not provide help in foreign languages.)

- [Add script file-download from URL](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Download_From_URL_EN.md) (download and store the script in ʻiCloud`)

- Local script (add script via UI method)

  - [Add local path script](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Local_JaveScript_EN.md) (Select `Local` as the script location, need to match [Add script file-from URL Download](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Download_From_URL_EN.md) tutorial study)
  
  - [Add remote link script](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_JaveScript_EN.md) (Select `Remote` as the script location)
  
  - [Modify local script settings](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/JaveScript_Modify_EN.md) (Modify local script alias, cron expression, script location, etc. series of operations)

- Subscription script (lazy artifact)

  - [URL requirements and content format requirements in the subscription script](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Script_Format_EN.md) (a must-see for newbies)

  - [Add subscription script](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Remote_Script_EN.md) (the role of the subscription script function, the link requirements and content requirements of the subscription URL)

  - [Create a single local branch](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Branch_EN.md) (Move the script in the subscription script to the local script, and you cannot modify the content of the local script. Only cron expressions can be modified)
  
  - [Create a single local branch and copy js](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Branch&Copy_EN.md) (Move the script in the subscription script to the local script, you can modify the script Content, cron expression can also be modified)

#### DNS

- [DNS](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/DNS_EN.md)

#### MITM

- [MITM](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/MITM_EN.md) (Man in the middle attack)

- [Hostname](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/hostname_EN.md) (two ways to add a hostname)

- [Certificate Management](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/CA_EN.md) (causes and solutions about certificate pop-ups appear)

#### Edit

- [Text Edit](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Configuration_EN.md) (Loon’s configuration file)

- [Download from URL](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/URL_Download_EN.md) (Download a complete set of configuration files from URL)

#### More

- [Network Sharing](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/Network_Sharing_EN.md) (Scientific Internet access can be achieved for devices under the same WiFi)

- [URL Schemes](https://github.com/TiyNa/LoonManual/blob/main/Plus_EN/URL_Schemes_EN.md)

---

### Author STATEMENT

- For the convenience of readers, it is forbidden to forward this tutorial **LINK** or **CONTENT** to any social platform in the mainland. If found, chiupam will delete the library for processing

- In the course of writing tutorials, please go to the [Telegram Loon official group](https://t.me/Loon0x00) and @[chiupam](https://t.me/chiupam) if there are really highly demanded tutorials. Chiupam will Schedule time to speed up writing tutorials

- Non-professionals, if the user still cannot solve the user's problem after consulting the tutorial, they can go to [Telegram Loon Official Group](https://t.me/Loon0x00) and have a friendly exchange

- Energy is limited, compiling tutorials voluntarily, it is impossible to update the tutorials that users need in real time

- With limited intelligence, it is impossible to write such tutorials for problems that cannot be solved by oneself
