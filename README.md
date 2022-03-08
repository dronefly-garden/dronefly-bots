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
    - to persistently set the bot status: `,botstatus playing online ,help for help`
- **cleanup** core (requires Manage Messages permission)
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

- **inatcog** repo: Dronefly-dpy2 https://github.com/dronefly-garden/dronefly dpy2
- **botstatus** repo: Dav-Cogs https://github.com/Dav-Git/Dav-Cogs
- **converters** repo: predacogs https://github.com/PredaaA/predacogs
    - not in use on Dronefly; testing for Dumbo
    - has a feat/dpy-2 branch but with minimum version 3.5.0 (SeedWasp currently at 3.5.0.dev1 which is lower)
    - the version on master seems fine, though
- **downloader** core
- **embedutils** repo: phen-cogs-dpy2 https://github.com/phenom4n4n/phen-cogs dpy2
- **weather** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
    - not in use on Dronefly; testing for Dumbo

### Dumbo

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public:** no
- **Purpose:** general purpose server info and management
- **Prefixes:** `-`

### Pickerel

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** audio
- **Prefixes:** `$`

### CuckooBee

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** development
- **Prefixes:** `c.`
