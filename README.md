# dronefly-bots
Red DiscordBot configurations for Dronefly and associated bots

## Bot configurations

### Dronefly

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public:** no (but invites may be available on request)
- **Purpose:** use naturalist-related infosystems: iNaturalist, eBird, etc.
- **Prefixes:** `,`

#### cogs

- **botstatus** repo: Dav-Cogs https://github.com/Dav-Git/Dav-Cogs
- **cleanup** core
- **commandstats** repo: Flare-Cogs https://github.com/flaree/Flare-Cogs
- **downloader** core
- **ebirdcog** repo: Dronefly
- **embedutils** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **extendedmodlog** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **fifo** repo: Fox-V3 https://github.com/bobloy/Fox-V3
- **inatcog** repo: Dronefly https://github.com/dronefly-garden/dronefly
- **modlog** core
- **permissions** core
- **retrigger** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **rss** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
- **rssnotifier** repo: JackCogs https://github.com/jack1142/JackCogs
- **say** repo: Laggrons-Dumb-Cogs https://github.com/laggron42/Laggrons-Dumb-Cogs
- **serverstats** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **tags** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **welcome** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/

### SeedWasp

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public:** no
- **Purpose:** test instance for Red-DiscordBot 3.5 / discord.py 2.0 migration
- **Prefixes:** `w,`

#### cogs

- **botstatus** repo: Dav-Cogs-red35 https://github.com/Dav-Git/Dav-Cogs red3.5
- **cleanup** core
- **commandstats** repo: Flare-Cogs-dpy2 https://github.com/flaree/Flare-Cogs dpy2
    - currently won't install (Flare has it locked to 3.4)
- **converters** repo: predacogs-dpy2 https://github.com/PredaaA/predacogs feat/dpy-v2
    - not in use on Dronefly; testing for Dumbo
- **downloader** core
- **ebirdcog** repo: Dronefly-dpy2
    - currently doesn't load properly (add_cog not awaited); disabled
- **embedutils** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **extendedmodlog** repo: Trusty-cogs-dpy2 https://github.com/TrustyJAID/Trusty-cogs dpy-2.0
- **inatcog** repo: Dronefly-dpy2 https://github.com/dronefly-garden/dronefly dpy2
- **modlog** core
- **permissions** core
- **retrigger** repo: Trusty-cogs-dpy2 https://github.com/TrustyJAID/Trusty-cogs dpy-2.0
- **rss** repo: aikaterna-cogs-dpy2 https://github.com/aikaterna/aikaterna-cogs v3_dpy2.0
- **rssnotifier** repo: JackCogs https://github.com/jack1142/JackCogs
    - currently doesn't load properly (add_cog not awaited); disabled
- **say** repo: Laggrons-Dumb-Cogs-dpy2 https://github.com/laggron42/Laggrons-Dumb-Cogs dpy2.0
- **serverstats** repo: Trusty-cogs-dpy2 https://github.com/TrustyJAID/Trusty-cogs dpy-2.0
- **tags** repo: phen-cogs-dpy2 https://github.com/phenom4n4n/phen-cogs dpy2
- **weather** repo: Trusty-cogs-dpy2 https://github.com/TrustyJAID/Trusty-cogs/ dpy-2.0
    - not in use on Dronefly; testing for Dumbo
- **welcome** repo: Trusty-cogs-dpy2 https://github.com/TrustyJAID/Trusty-cogs/ dpy-2.0

### Dumbo

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public:** no
- **Purpose:** general
- **Prefixes:** `-`

#### cogs

- **botstatus** repo: Dav-Cogs https://github.com/Dav-Git/Dav-Cogs
- **cleanup** core
- **commandstats** repo: Flare-Cogs https://github.com/flaree/Flare-Cogs
- **downloader** core
- **converters** repo: predacogs https://github.com/PredaaA/predacogs
- **dalle** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
- **dictionary** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
- **downloader** core
- **embedutils** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **eventposter** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **extendedmodlog** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **fifo** repo: Fox-V3 https://github.com/bobloy/Fox-V3
- **general** core
- **modlog** core
- **permissions** core
- **randimals** repo: tmerc-cogs https://github.com/tmercswims/tmerc-cogs
- **reactpoll** repo: FlapJack-Cogs https://github.com/flapjax/FlapJack-Cogs
- **reacttickets** repo: SauriCogs https://github.com/elijabesu/SauriCogs
- **remindme** repo: PCXCogs https://github.com/PhasecoreX/PCXCogs
- **retrigger** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **say** repo: Laggrons-Dumb-Cogs https://github.com/laggron42/Laggrons-Dumb-Cogs
- **seen** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
- **serverstats** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **simplecalculator** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **strawpoll** repo: Sharky https://github.com/SharkyTheKing/Sharky
- **tags** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **timezone** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
- **trivia** core
- **tweets** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **weather** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **wikipedia** repo: PCXCogs https://github.com/PhasecoreX/PCXCogs

### Pickerel

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** audio
- **Prefixes:** `$`

#### cogs

- **audio** core
- **botstatus** repo: Dav-Cogs https://github.com/Dav-Git/Dav-Cogs
- **downloader** core
- **permissions** core

### Polistes

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** admin
- **Prefixes:** `;`

#### cogs

- **admin** core
- **cleanup** core
- **deleter** repo: Toxic-Cogs https://github.com/NeuroAssassin/Toxic-Cogs
- **botstatus** repo: Dav-Cogs https://github.com/Dav-Git/Dav-Cogs
- **downloader** core
- **extendedmodlog** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **lockdown** repo: palmtree5-cogs https://github.com/palmtree5/palmtree5-cogs redv3-rewrites
- **mod** core
- **modlog** core
- **permissions** core
- **roleutils** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
- **serverstats** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **stickyroles** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
- **warnings** core

### CuckooBee

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** development
- **Prefixes:** `c.`

#### cogs

- misc. as needed to do do development for each of the bots above
