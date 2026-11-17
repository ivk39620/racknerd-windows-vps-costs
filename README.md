# Windows VPS USA: What RackNerd's $10.60/Year Entry Really Costs With Windows, Which Tier Fits MT4 or a Small RDP Team, and Why a US IP Can Move Under You (Full Plan Table)

RackNerd's US KVM plans start at $10.60/year for 1GB and top out at $62.49/year for 8GB, and none of those prices include a Windows Server licence. In the US market a licensed Windows box is usually billed as a separate line at around $20/month, so the yearly plans on this list are a cheap route to a US server, not automatically a cheap route to a US Windows desktop. What follows covers all twelve current plans, the licence math that decides your real annual cost, how many people can share one box before you owe Microsoft more money, which Windows versions are worth installing in late 2026, and an IP-stability issue in Los Angeles that matters if a trading platform or marketplace whitelists your address.

> **Most readers:** the 4GB annual special at $29.98/year (3 vCPU, 4GB RAM, 65GB SSD, 6.5TB transfer) is the smallest tier that runs Windows Server with room for updates plus one real application, and it assumes you bring the licence. One or two people sharing it need no extra licensing. 👉 [See RackNerd's current US plan list and live prices](https://bit.ly/RacKnerd)

## What RackNerd actually sells in the US

Twelve KVM plans, split between a standard line and four promotional annual tiers. The standard line scales from 512MB to 12GB; the annual specials are cheaper per gigabyte but come with smaller disks and are the ones that sell out.

| Plan | vCPU / RAM / SSD | Transfer | Price (yearly) | Order |
| --- | --- | --- | --- | --- |
| 512MB KVM | 1 core / 512MB / 30GB | 500GB | $26.99/yr | [Order the 512MB plan](https://bit.ly/RacKnerd) |
| 1GB KVM | 2 cores / 1GB / 50GB | 1TB | $17.99/yr | [Order the 1GB standard plan](https://bit.ly/RacKnerd) |
| 2GB KVM | 3 cores / 2GB / 75GB | 2TB | $20.59/yr | [Order the 2GB plan](https://bit.ly/RacKnerd) |
| 4GB KVM | 4 cores / 4GB / 130GB | 3TB | $24.59/yr | [Order the 4GB standard plan](https://bit.ly/RacKnerd) |
| 6GB KVM | 5 cores / 6GB / 170GB | 4TB | $27.59/yr | [Order the 6GB standard plan](https://bit.ly/RacKnerd) |
| 8GB KVM | 6 cores / 8GB / 220GB | 5TB | $36.59/yr | [Order the 8GB standard plan](https://bit.ly/RacKnerd) |
| 12GB KVM | 7 cores / 12GB / 300GB | 6TB | $55.99/yr | [Order the 12GB plan](https://bit.ly/RacKnerd) |
| 1GB KVM annual special | 1 core / 1GB / 25GB | 2TB | $10.60/yr | [Order the 1GB annual special](https://bit.ly/RacKnerd) |
| 2.5GB KVM annual special | 2 cores / 2.5GB / 45GB | 3TB | $18.66/yr | [Order the 2.5GB annual special](https://bit.ly/RacKnerd) |
| 4GB KVM annual special | 3 cores / 4GB / 65GB | 6.5TB | $29.98/yr | [Order the 4GB annual special](https://bit.ly/RacKnerd) |
| 6GB KVM annual special | 5 cores / 6GB / 100GB | 10TB | $44.98/yr | [Order the 6GB annual special](https://bit.ly/RacKnerd) |
| 8GB KVM annual special | 6 cores / 8GB / 150GB | 20TB | $62.49/yr | [Order the 8GB annual special](https://bit.ly/RacKnerd) |

Two things in that table are worth pointing out because they look like typos. The 512MB plan at $26.99/year costs more than the 1GB annual special at $10.60/year, so nobody should buy the smaller one. And the 2.5GB special at $18.66 sits below the 4GB standard at $24.59 with the same amount of RAM headroom for Windows, which makes the special the better buy if you can live with 45GB of disk. Promotions on this lineup rotate; the order page shows the live figure and the billing term for each tier.

## The licence is the real decision: $30/year vs about $270/year

Windows Server licensing is the part of a "cheap Windows VPS" that the headline price leaves out, and two US providers spell out the arithmetic.

GigeNET charges a flat **$20.28/month** for Windows Server Standard on every plan, so its $35 four-gigabyte plan is really **$55.28/month**, and a bigger plan is simply the plan price plus the same $20.28. HostFinch lists Windows Server 2019 and 2016 Standard as a **$19.99/month** checkout add-on, which turns its $12.99 plan into **$32.98/month**. Kamatera takes the other approach and states that any operating system costs the same, Windows included.

Two models, same market, roughly $20/month of difference in how the bill is presented. $20/month is $240 a year.

RackNerd's published plan list prices the server only. There is no Windows Server line item anywhere in it, which normally means one of two things: you supply a licence you're entitled to use, or the provider won't hand you a licensed Windows image at all. Ask support before you pay, and ask specifically whether they will activate a Windows ISO you provide. If the answer is yes, your 4GB annual special becomes roughly $30 plus a licence you already own. If the answer is no, the cheap tier stops being a Windows option and the comparison moves to providers that bundle it.

👉 [Confirm the Windows licence question before you check out](https://bit.ly/RacKnerd)

## Sharing the desktop: two sessions free, then CALs

Windows Server allows **two administrator sessions at once** without any extra licensing, which covers a solo trader running MT4 or MT5, or two people remote-desktoping into the same accounting machine. This is where a $30/year box genuinely competes with a $55/month one.

The third concurrent user changes the math. GigeNET sells Remote Desktop CALs at **$7.50/month each**, or **$35/month for a five-pack**, and its remote desktop plans include them. HostFinch quotes CALs on request without a public price. Five people sharing one Windows box therefore add $35/month to whatever the server costs, which is more than a year of the RackNerd 8GB plan. Size the box by concurrent users, not by core count: CALs are a per-person cost and cores don't reduce it.

👉 [Compare the 6GB and 8GB tiers for multi-user work](https://bit.ly/RacKnerd)

## Which Windows version you end up with

The version matters more right now than it usually does, because **Windows Server 2016 reaches the end of Microsoft's security updates on January 13, 2027**, about two months from now, while **Windows Server 2019 runs to January 10, 2029**. Those are Microsoft's own support dates, and GigeNET prints both on its product page along with a blunt recommendation to pick 2019.

The pattern across the market: the cheapest tiers are the ones still offering 2016. GigeNET offers 2016 and 2019 and pushes 2022 and 2025 to dedicated servers on request. HostFinch lists 2016 and 2019, with 2022 by quote. IONOS offers only 2022 or 2025. Infrawire goes wider, from 2025 down to 2012 plus Windows 11 and 10 desktop images.

If you bring your own licence, the version is your choice and the only cost of picking 2019 over 2016 is nothing. If the provider supplies the licence, expect the bottom tier to mean the oldest image on the shelf. Installing 2016 in November 2026 buys you a server that stops receiving security patches within weeks of setup.

## How much RAM Windows needs before plan size matters

Windows Server needs **at least 2GB of RAM and 20GB of disk**, and GigeNET's order form enforces that, which is why its lineup starts at 4GB. The provider's own guidance is to take 4GB or more because updates, a browser and one real application will eat past 2GB, and **8GB or more for SQL Server or several RDP users**.

Applied to RackNerd: the $10.60 1GB special and the $18.66 2.5GB special are Linux territory. 4GB is the practical floor for a Windows desktop, 6GB is comfortable for a line-of-business app with a database, and 8GB is where multi-user sessions and SQL Express stop swapping. Disk matters too: 65GB on the 4GB special leaves about 45GB for Windows and your software after the OS install, which is enough for QuickBooks, Sage 50 or an MT4 setup with history, and tight for anything that accumulates logs.

## The US IP problem nobody mentions

A US IP is often the whole reason for buying: platforms that only accept US connections, marketplace seller tools, broker APIs, ad accounts. That makes IP stability part of the product, and RackNerd's Los Angeles footprint has been moving.

RackNerd's own maintenance notice, as published in November 2026 coverage, states that its upstream colocation provider exited the 707 Wilshire Blvd facility, requiring hardware to be physically moved from Los Angeles DC-02 to DC-03 at 1200 W 7th St, with **mandatory IP address changes** for affected services because DC-03 runs on different network infrastructure (AS36352). An earlier 2023 renumbering at the same facility had already replaced addresses across the LA datacenter.

For a hobby site this is an afternoon of DNS. For a trading bot tied to a whitelisted IP, or a marketplace account that flags a login from a new address, it's a support ticket and a re-verification. If your use case locks onto a specific IP, keep a second address or a second provider in reserve, and treat any single cheap US VPS as replaceable infrastructure.

## How RackNerd compares on Windows pricing

| Provider | Windows pricing model | Entry figure | Notes |
| --- | --- | --- | --- |
| GigeNET | Licence billed separately, flat $20.28/mo | $55.28/mo all-in for 4GB / 90GB SSD / 5TB | Chicago, Ashburn, Los Angeles; hourly or monthly billing; page dated 2026-10-17 |
| HostFinch | Licence as a $19.99/mo checkout add-on | $12.99/mo plan, $32.98/mo with Windows | 1 vCPU / 2GB / 40GB, unmetered traffic; page dated 2026-09-26 |
| Kamatera | Bundled, any OS at the same price | 30-day trial up to $100 of configuration plus 1TB traffic, card required | 8 US locations; trial converts to paid if you don't terminate; page dated 2026-03-24 |
| Infrawire | Bundled | From €8.30/mo in New York | 10Gbps port, NVMe, 7-day money-back guarantee; priced in euros; page dated 2026-03-26 |
| RackNerd | No licence in the plan list | $29.98/yr for 4GB / 65GB SSD, licence separate | US KVM plans from $10.60/yr; confirm licence handling with support before ordering |

The euro figure isn't comparable to the dollar ones without a conversion, and the four pages were captured across eight months, so treat this as a map of pricing models rather than a single price ranking.

## Which tier for which job

**One person, MT4/MT5, NinjaTrader or an automation script.** 4GB annual special at $29.98. Two cores would do, but Windows plus a trading terminal plus a chart-heavy setup wants the headroom, and the next step up costs $15 more a year.

**One or two people remote-desktoping into an office machine for QuickBooks, Sage 50 or an ERP client.** 6GB annual special at $44.98. No CALs needed at two users; the extra RAM is for the app and the database file, not for the sessions.

**Five or more concurrent RDP users.** Skip the small tiers. 8GB annual at $62.49 plus five CALs at roughly $35/month from a provider that sells them, or a provider whose plan already includes them. The licensing overtakes the server cost at this point.

**SQL Server, IIS or a .NET line-of-business app.** 8GB or above. GigeNET's own split puts SQL Express and busier IIS sites on 8 cores and 8GB, and larger databases on 16GB. Also worth checking whether the app really needs Windows: modern .NET runs on Linux, and paying for a Windows licence to host something that doesn't need it is the most common waste in this category.

**A US IP for a platform that only accepts US connections.** Any tier works, but read the section above on IP churn first and plan for the address to change at least once.

## FAQ

**Does RackNerd include a Windows Server licence?**
Nothing in its published plan list prices one. Ask support whether they will activate a Windows image you supply, and get the answer in writing before you order. If they won't, budget the market rate of roughly $20/month for a licensed Windows box elsewhere.

**Do two people sharing one Windows VPS need CALs?**
No. Windows Server includes two concurrent administrator sessions, which covers a pair of users. The third concurrent user is where CALs start, at around $7.50/month each.

**Can a $10.60/year plan run Windows?**
Not realistically. Windows Server needs 2GB of RAM minimum and 4GB to be usable alongside updates and an application, so the 1GB and 2.5GB tiers are for Linux.

**Why would my US IP change after I buy?**
Facility moves and upstream network changes force renumbering. RackNerd's Los Angeles DC-02 to DC-03 relocation came with mandatory IP changes for affected services. Any provider can do this; the ones that communicate it early are easier to plan around.

## Before you order

Match the tier to the licence, not the other way around. If you own a Windows Server licence you're entitled to use and you need one or two RDP sessions, the 4GB annual special at $29.98 is the cheapest sane entry and the 6GB at $44.98 is the comfortable one. If you need the provider to hand you a licensed Windows box, add about $20/month to whatever the server costs, or pick a provider that bundles it and compare the all-in figure instead.

Three things to confirm on the order page before paying: whether a Windows licence is included or accepted, which Windows versions are offered (anything below 2019 is a countdown to January 2029, and 2016 stops updating on January 13, 2027), and the renewal price for the tier you picked, since promotional annual plans renew at whatever the list price is at the time.

👉 [Open RackNerd's current US plan list and check stock](https://bit.ly/RacKnerd)
