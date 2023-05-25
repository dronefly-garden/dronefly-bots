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
    - currently installed from my PR supporting red 3.5:
      https://github.com/synrg/Fox-V3 PR-fifo-firstmessage-red3.4+3.5
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
    - currently installed from Laggron's `dpy2.0` branch to support red 3.5
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

- every cog that is on Dronefly is also on SeedWasp from the same repos.
- additionally, SeedWasp has `weather` and `wikipedia`
    - a perk for servers that have invited this instance instead of Dronefly
    - see Dumbo's cogs for details

### Dumbo

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public:** no
- **Purpose:** general
- **Prefixes:** `-`

#### cogs

- selected cogs that are also on Dronefly or SeedWasp (same versions):
  `botstatus cleanup commandstats downloader embedutils extendedmodlog`
  `fifo modlog permissions retrigger say serverstats tags weather`    
- plus additional cogs listed below
- **aiart** repo: kaogurai-cogs https://github.com/kaogurai/cogs
    - whole cog is disabled by default
    - currently in evaluation on one server, on which many commands are disabled because they didn't produce useful results, or else produced largely nsfw images
- **converters** repo: predacogs https://github.com/PredaaA/predacogs
    - numerous conversions provided via `-conv` command, e.g.
        - `-conv c f 0` to convert 0C to 32F
        - `-conv c f 32` to convert 32F to 0C
- **dictionary** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
    - `-define` command providing basic dictionary lookup
- **editor** repo: Toxic-Cogs https://github.com/NeuroAssassin/Toxic-Cogs
    - `-editmessage` command to edit a message the bot sent
- **firstmessage** repo: Fox-V3 https://github.com/bobloy/Fox-V3
    - currently installed from my PR supporting red 3.5:
      https://github.com/synrg/Fox-V3 PR-fifo-firstmessage-red3.4+3.5
- **general** core
    - various toy or useful commands
    - `-help General` for a list of all commands
- **randimals** repo: tmerc-cogs https://github.com/tmercswims/tmerc-cogs
    - various random animal images
    - `-help Randimals` for a list of all commands
- **remindme** repo: PCXCogs https://github.com/PhasecoreX/PCXCogs
    - `-remindme` to send user a reminder relative to the current time
- **seen** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
    - `-seen <user>` to report when they were last seen in chat
- **simplecalculator** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
   - `-calc` to perform basic math calculations
- **timezone** repo: aikaterna-cogs https://github.com/aikaterna/aikaterna-cogs
   - `-time me` to show or set your current time zone
   - `-time compare <user>` to compare your time to another user's time in their time zone
- **trivia** core
   - set up on `#trivia` channel in iNat Discord server; instructions are pinned
- **weather** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
   - `-weather` (alias `-we`) provides crowdsourced weather current conditions and forecasts from openweathermap.org
   - registered with Ben's API key, providing up to 1,000 weather API calls per day free and up to $1.50 per day for an additional 1K calls to a max of 2K
   - we don't expect to ever have to dip into the paid limit - if we're wrong about that, we may have to reevaluate offering this one
- **wikipedia** repo: PCXCogs https://github.com/PhasecoreX/PCXCogs
   - `-wiki` to perform Wikipedia.org lookups

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

- apart from a handful of standard cogs on the other bots, the special-purpose admin bot cogs below
- **admin** core
    - various commands for server administration
    - `;help Admin` to list them all
- **deleter** repo: Toxic-Cogs https://github.com/NeuroAssassin/Toxic-Cogs
    - `;deleter channel` to set a channel's automatic message deletion period
    - automatically deletes old messages in modlog channels and trivia so the server doesn't accumulate a large number of transient messages with low or negative value to retain
    - each channel has the retention period stated in the channel description
- **lockdown** repo: palmtree5-cogs https://github.com/palmtree5/palmtree5-cogs redv3-rewrites
    - `;lockdown` to implement server lockdown - see Mod guide document for details (private Google doc)
- **mod** core
    - various commands for server moderation
    - `;help Mod` to list them all
- **roletools** repo: Trusty-cogs https://github.com/TrustyJAID/Trusty-cogs/
    - make roles sticky, create dropdown and button menus
    - `;help RoleTools` to list all commands
- **roleutils** repo: phen-cogs https://github.com/phenom4n4n/phen-cogs
    - commands to create reaction role menus, etc.
    - on iNat server, `roletools` cog is now preferred
    - `;help RoleUtils` to list all commands
- **slowmode** repo: palmtree5-cogs https://github.com/palmtree5/palmtree5-cogs redv3-rewrites
    - `;toggleslow` to implement slowmode
- **warnings** core
    - `;warn` to warn a user
    - other commands to view & maintain a warnings list, as well as perform automatic actions
    - `;help Warnings` to list them all

### CuckooBee

- **Operator:** `@SyntheticBee` on Discord (GitHub: @synrg)
- **Public: no**
- **Purpose:** development
- **Prefixes:** `c.`

#### cogs

- misc. as needed to do do development for each of the bots above
