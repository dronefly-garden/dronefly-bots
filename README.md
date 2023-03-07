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
- **cleanup** core (requires Manage Messages permission)
    - to persistently set the bot status: `,botstatus playing online ,help for help`
- **commandstats** repo: Flare-Cogs https://github.com/flaree/Flare-Cogs
- **downloader** core
- **ebirdcog** repo: Dronefly https://github.com/dronefly-garden/dronefly
- **embedutils** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
    - `,embed global list` for global embeds and `,embed show` to show
    - `bonapkey` and `mapkey` show keys for bonap and iNat maps, respectively
- **extendedmodlog** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
    - shunt command logging to a specific mods-only channel
- **fifo** repo: Fox-V3 https://github.com/bobloy/Fox-V3
    - on selected servers to schedule detailed `,ebird hybrids` command execution in a specific channel for a specific location
- **inatcog** repo: Dronefly https://github.com/dronefly-garden/dronefly
    - configured by:
        - admins: `,inat set`
        - member managers: `,user add`
        - any user registered by a member manager: `,place add`, `,project add`
        - any registered user (self-registered *or* mod-registered): `,user set`
- **modlog** core
- **permissions** core
- **retrigger** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
    - experimental retrigger `,tbird` executes both the `,t` command and `,xcsp` on the same taxon query
- **rss** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
    - can be used to subscribe to user and project journals
    - e.g.
        - `,rss add benarmstrong #bot-testing https://www.inaturalist.org/journal/benarmstrong.atom`
        - `,rss add fly-guide #bot-testing https://www.inaturalist.org/projects/flies-of-the-us-and-canada/journal.atom`
    - `,rss list` to list configuration
- **rssnotifier** repo: JackCogs https://github.com/jack1142/JackCogs
    - can be used to ping a specific role when a feed is updated, e.g.
        - `,rssnotifier addroles fly-guide #bot-testing FliNat`
- **say** repo: Laggrons-Dumb-Cogs https://github.com/retke/Laggrons-Dumb-Cogs
    - can be used to make Dronefly "speak" in another channel, e.g.
        - `,say #chat Feed me.`
- **serverstats** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
    - `inatcog` dispatches `commandstats_action` events for `,taxon` display reaction buttons:
        - `react taxonomy`, `react self`, `react user`, `react home`, `react place`
    - these reactions are counted in `,cmd` output (owner only)
- **tags** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
    - `,tags` to show all tags
    - see: https://dronefly.readthedocs.io/en/latest/guide_for_participants.html#dronefly-custom-commands
- **welcome** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
    - see `,help welcomeset` for help setting up

### SeedWasp

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public:** no
- **Purpose:** test instance for Red-DiscordBot 3.5 / discord.py 2.0 migration
- **Prefixes:** `w,`

See https://github.com/dronefly-garden/dronefly-bots/issues/1 for a more thorough accounting of work-in-progress to bring SeedWasp to a state where it uses everything that Dronefly does, with all of it supported on discord.py 2.0.

#### cogs

- **botstatus** repo: Dav-Cogs-red35 https://github.com/Dav-Git/Dav-Cogs red3.5
- **cleanup** core
- **commandstats** repo: Flare-Cogs-dpy2 https://github.com/flaree/Flare-Cogs dpy2
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
- **wikipedia** repo: PCXCogs https://github.com/PhasecoreX/PCXCogs
    - using my fork for now until my PR is merged: https://github.com/synrg/PCXCogs
    - https://github.com/PhasecoreX/PCXCogs/pull/101

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
- **toggleslow** repo: palmtree5-cogs https://github.com/palmtree5/palmtree5-cogs redv3-rewrites
- **warnings** core

### CuckooBee

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** development
- **Prefixes:** `c.`

#### cogs

- misc. as needed to do do development for each of the bots above
