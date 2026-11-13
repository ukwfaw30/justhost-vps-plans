# VPS Linux guide: which JustHost plan fits a blog, WordPress or a database, and what you pay monthly vs on a 12-month prepay (full price list)

Most people shopping for a cheap Linux VPS should start with **New Star**: 1 vCPU, 1 GB RAM, 10 GB NVMe and a 100 Mbps unmetered port, listed at **$3.81/month**, or **$3.05/month** effective if you pay for 12 months at once. That covers a static site, a cached WordPress install, a WireGuard node or a monitoring agent. If your application and MySQL have to share one machine, start at 2 GB instead.

Below are the plans in JustHost's current price list, the two upgrades on that list that are worth the money, the pairs of plans that quietly duplicate each other, and the four questions the price list leaves open: backups, downgrades, cancellation terms and managed support.

> **Quick pick for most readers:** New Star, $3.81/mo, or $3.05/mo on a 12-month prepay, for one small site or service. 👉 Check New Star's current configuration and price

## JustHost's Linux VPS plans and prices

Nine named NVMe plans run from $1.99 to $18.30 a month. They are KVM virtual machines with an unmetered port at the speed shown, and DDoS protection against the main attack types is included. The traffic figure in brackets is JustHost's own conversion of the port speed into a monthly volume.

| Plan | vCPU / RAM / NVMe | Port (traffic equivalent) | Monthly | 12-month prepay | Order |
| --- | --- | --- | --- | --- | --- |
| VPS Promo | 1 / 512 MB / 5 GB | 10 Mbps (4+ TB/mo) | $1.99 | not shown | [ Order VPS Promo](https://justhost.asia/en/services/vps/tariffs/promo-c1r512nvme?ref=196392) |
| New Star | 1 / 1 GB / 10 GB | 100 Mbps (31+ TB/mo) | $3.81 | $3.05 | [ Order New Star](https://justhost.asia/en/services/vps/tariffs/new-star-c1r1024nvme?ref=196392) |
| Sirius | 1 / 1 GB / 20 GB | 300 Mbps (93+ TB/mo) | $4.85 | $3.88 | [ Order Sirius](https://justhost.asia/en/services/vps/tariffs/sirius?ref=196392) |
| Arcturus | 1 / 2 GB / 30 GB | 300 Mbps (93+ TB/mo) | $6.92 | $5.53 | [ Order Arcturus](https://justhost.asia/en/services/vps/tariffs/arcturus?ref=196392) |
| Double Star | 2 / 2 GB / 20 GB | 200 Mbps (62+ TB/mo) | $7.08 | $5.67 | [ Order Double Star](https://justhost.asia/en/services/vps/tariffs/double-star-c2r2048nvme?ref=196392) |
| Alpha Centauri | 2 / 2 GB / 40 GB | 400 Mbps (124+ TB/mo) | $8.99 | $7.19 | [ Order Alpha Centauri](https://justhost.asia/en/services/vps/tariffs/alpha_centauri?ref=196392) |
| Bright Star | 4 / 4 GB / 30 GB | 300 Mbps (93+ TB/mo) | $9.80 | $7.84 | [ Order Bright Star](https://justhost.asia/en/services/vps/tariffs/bright-star-c4r4096nvme?ref=196392) |
| Vega | 2 / 4 GB / 80 GB | 500 Mbps (155+ TB/mo) | $13.44 | $10.75 | [ Order Vega](https://justhost.asia/en/services/vps/tariffs/vega?ref=196392) |
| Capella | 4 / 4 GB / 120 GB | 750 Mbps (232+ TB/mo) | $18.30 | $14.64 | [ Order Capella](https://justhost.asia/en/services/vps/tariffs/capella?ref=196392) |

Three things to know before you read those numbers:

- The 12-month column is the effective monthly rate when you prepay a year, which takes 20% off. Monthly billing costs the list price.
- New Star, Double Star and Bright Star are listed as available when you order three months or more.
- JustHost's VPS overview page carries "Special" versions of Sirius, Arcturus and Vega at $2.81, $4.01 and $7.79 a month for identical specifications. Those read like limited offers. Take the lower number if checkout shows it, but don't build a budget around it.

The range continues above Capella with 4 cores/8 GB/200 GB, 6 cores/12 GB/400 GB and 8 cores/24 GB/600 GB. The overview page lists those at $16.20, $26.40 and $47.40 a month ($12.96, $21.12 and $37.92 on annual prepay) under the names Yildun, Betelgeuse and Altair.

JustHost also sells storage-selectable configurations under the VPS Start, Standard and Super names in HDD, SSD or NVMe, plus IPv6-only machines from $1.60 a month. An IPv6-only box is only useful if everything that connects to it speaks IPv6, which rules out most home connections and a fair number of monitoring tools.

## Two upgrades worth paying for, and two plans that duplicate each other

New Star to Sirius costs $1.04 more and doubles NVMe from 10 GB to 20 GB while tripling the port from 100 Mbps to 300 Mbps. For a site that serves images or runs regular updates, it's the cheapest meaningful step on the list.

Sirius to Arcturus costs $2.07 and doubles RAM to 2 GB, with 10 GB more disk. This is the step that lets MySQL and PHP share a box without swapping.

Then the ladder gets uneven. Double Star ($7.08, 2 cores/2 GB/20 GB, 200 Mbps) sits $1.91 below Alpha Centauri ($8.99, 2 cores/2 GB/40 GB, 400 Mbps). Same cores, same RAM, and Alpha Centauri doubles disk and port for less than two dollars. Double Star only wins if that $1.91 is the entire budget.

Bright Star ($9.80, 4 cores/4 GB/30 GB, 300 Mbps) against Vega ($13.44, 2 cores/4 GB/80 GB, 500 Mbps): Vega costs $3.64 more and halves your core count. Buy Vega when 80 GB of disk is the actual requirement, not as a general upgrade. Capella ($18.30, 4 cores/4 GB/120 GB, 750 Mbps) is the first plan that adds cores and disk together.

👉 See the Alpha Centauri configuration and its current price

## How much server does your project need?

For scale, Reg.ru's smallest Linux VPS is 1 core/1 GB/10 GB SSD at 390 ₽ a month. Contabo's entry configuration is 4 vCPU/8 GB/100 GB SSD at €5.50 a month for the first 24 months. Atlantic.Net's General Purpose G3.2GB (1 vCPU, 2 GB, 50 GB, 3 TB) is $8.00 a month. Same product category, very different amounts of hardware for the money.

- **Static site, blog with a caching plugin, VPN endpoint, uptime monitor:** 512 MB to 1 GB is honest here. VPS Promo at $1.99 or New Star at $3.81.
- **One WordPress site with WooCommerce and a real database:** 2 GB. Arcturus ($6.92, 30 GB) if the catalogue has images; Alpha Centauri ($8.99, 40 GB) if you also want the faster port.
- **LAMP or LEMP application with MySQL on the same machine:** 2 cores and 2 GB at minimum. Alpha Centauri.
- **Docker host, GitLab runner, CI jobs:** cores matter more than disk. Bright Star's 4 cores at $9.80.
- **A database that grows, or local backups:** disk matters more than cores. Vega's 80 GB, Capella's 120 GB.
- **More than 4 GB of RAM:** JustHost starts at $16.20 there, and Contabo sells 8 GB for less per gigabyte. Compare port speed and minimum term rather than the headline price.

## What "unmetered port" means on these plans

JustHost sells bandwidth as port speed rather than as a monthly quota: 10 Mbps to 750 Mbps, marked fair-share. The TB figure in the table is what that port would move if it ran flat out for 30 days, so treat it as a ceiling, not an allowance. Fair-share means a neighbour saturating their port can affect yours at peak times. A website rarely notices; a nightly backup job that has to finish before morning sometimes does.

Competitors measure the same thing three different ways. OVHcloud advertises unlimited traffic with ports up to 3 Gbps depending on the model. Contabo pairs unlimited traffic with 200, 300, 600 or 800 Mbit/s ports depending on configuration. Liquid Web gives a fixed outbound allowance of 2 TB to 10 TB. An "unlimited" plan, a "750 Mbps fair-share" plan and a "5 TB" plan can't be compared on price alone.

## VPS Linux fine print: four things the price list doesn't answer

**Backups.** JustHost's price list doesn't publish a backup policy or a retention window, and that number decides whether a bad `rm` ruins your week. For reference, OVHcloud includes a daily automated backup with 24 hours of retention on every VPS and sells a Premium tier with 7-day retention. Liquid Web leaves backup configuration to you or to a separate Acronis licence. Atlantic.Net lists onsite and offsite backups as options. Ask support what your plan keeps and for how long before you migrate a live site.

**Downgrades.** Reg.ru spells out the trap: once you expand a disk, you can't return to the original plan. Assume shrinking is harder than growing everywhere, and buy the disk you'll need in six months rather than the one you need today.

**Cancellation and billing.** Contabo requires no minimum notice on prepaid terms and four weeks on postpaid. Reg.ru bills hourly with a 100 ₽ minimum payment and discounts 7–10% for monthly or longer terms. JustHost's 20% is tied to a 12-month prepay, so the commitment is a year of prepayment.

**Managed support.** All of the above are self-managed. If you want someone else to patch the OS and watch the graph, Liquid Web's fully managed entry plan (1 vCPU, 2 GB, 60 GB, 2 TB) starts at $11 a month with a 100% uptime guarantee. That premium buys administration, not hardware.

👉 Compare all JustHost VPS tariffs on one page

## Self-managed or fully managed

| Provider | Entry configuration | Price | Who administers it |
| --- | --- | --- | --- |
| JustHost | 1 vCPU / 1 GB / 10 GB NVMe | $3.81/mo ($3.05 on annual prepay) | You |
| Reg.ru | 1 core / 1 GB / 10 GB SSD | 390 ₽/mo | You |
| Contabo | 4 vCPU / 8 GB / 100 GB SSD | €5.50/mo for the first 24 months | You |
| Atlantic.Net | 1 vCPU / 2 GB / 50 GB, 3 TB | $8.00/mo | You |
| Liquid Web | 1 vCPU / 2 GB / 60 GB, 2 TB | $11/mo | The provider |

## FAQ

**Is 1 core and 1 GB of RAM enough?** For one low-traffic WordPress site with a caching plugin, a static site, a VPN node or a monitoring agent, yes. For MySQL plus an application server on the same box, no. Swap makes small instances survive; it doesn't make them fast.

**Monthly or 12 months upfront?** The 20% discount is the whole difference: New Star is $45.72 for a year billed monthly and $36.60 prepaid. Prepay only if you're confident the project outlives the year.

**Can I upgrade later without downtime?** OVHcloud advertises one-click upgrades with no downtime, and Liquid Web advertises scaling with virtually no downtime. JustHost doesn't document its upgrade path on the price list, so ask support before you pick a plan you intend to outgrow.

**Can I install Windows instead?** KVM-based platforms boot the images the provider offers, and a Windows licence is a separate cost from the server. Reg.ru has stopped selling Windows VPS altogether. If Windows is a hard requirement, confirm the template exists before paying.

**What does KVM change for me?** Each VM gets its own kernel, so you can load modules, run Docker or set up a custom firewall without the host kernel getting in the way. Reg.ru describes its KVM instances as behaving like a real physical server, which is the practical version of that claim.

## Before you order

Pick by workload: one small site or service, New Star. WordPress with a database and real traffic, Arcturus or Alpha Centauri. Docker or CI work, Bright Star. Past 4 GB of RAM, price Contabo's larger configurations before defaulting to JustHost's upper tiers.

Confirm three things at checkout: whether the figure shown already includes the 20% annual discount, whether your plan carries a three-month minimum, and what the backup retention is. Downgrades are usually one-way.

👉 Start with New Star at $3.81/mo, or $3.05/mo on a 12-month prepay
