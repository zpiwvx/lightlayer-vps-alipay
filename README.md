# VPS with Alipay Payment: What LightLayer Costs Now, Which Route Tier to Buy, and Whether You Can Get a Refund (Full Plan Table)

LightLayer accepts Alipay, doesn't ask for an international credit card, and its cheapest entry point is now **$5/month**. The $4 plan most write-ups still quote was discontinued on September 30, 2026. On annual billing, a 1 GB box with 50 GB NVMe runs **$24.99/year** in Manila or Taiwan, or **$49.99/year** in Los Angeles on the Premium CN2 route.

The rest of this page covers the full current lineup, what the three Los Angeles network tiers actually change, the monthly-to-annual math, and the refund rule that should decide whether you commit for a year.

> **Most people paying with Alipay here:** the 1 GB annual plan in Taiwan or Manila at $24.99/year if you just need a box that stays up, or Los Angeles Premium at $49.99/year if your users sit in mainland China. Prices are quoted in USD and Alipay settles the RMB side at its own rate.
>
> 👉 [See LightLayer's current plans and pay with Alipay](https://account.lightlayer.net/?affid=74)

## LightLayer's current plans and prices

The lineup splits into monthly cloud plans and per-location annual deals. All of it runs on KVM with AMD EPYC processors and NVMe storage.

**Monthly cloud plans**

| Plan | What you get | Price | Billing | Order |
| --- | --- | --- | --- | --- |
| Entry plan (LA, Global route) | 1 vCPU · 1 GB RAM · 50 GB NVMe · 100 Mbps unmetered | $5.00/mo | Monthly | [Order the entry plan](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Pay As You Go | 2+ vCPU · 2 GB+ RAM · scalable storage · 200 Mbps+ · Standard route | from $5.60/mo | Monthly | [Configure Pay As You Go](https://account.lightlayer.net/index.php?/cart/specialoffer/&affid=74) |
| Business | 32 vCPU · 32 GB RAM · scalable storage · 200 Mbps unmetered · Premium route | $53.60/mo | Monthly | [Order the Business plan](https://account.lightlayer.net/index.php?/cart/specialoffer/&affid=74) |

**Annual deals, all 1 vCPU / 1 GB RAM / 50 GB NVMe**

| Location and route | Price | Billing | Order |
| --- | --- | --- | --- |
| Manila (Premium, Standard or Global) | $24.99/yr | Annual | [Order Manila annual](https://account.lightlayer.net/index.php?/cart/manila/&affid=74) |
| Taiwan (Premium, Standard or Global) | $24.99/yr | Annual | [Order Taiwan annual](https://account.lightlayer.net/index.php?/cart/taiwan/&affid=74) |
| Los Angeles, Global | $29.99/yr | Annual | [Order LA Global](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Los Angeles, Standard | $39.99/yr | Annual | [Order LA Standard](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |
| Los Angeles, Premium (CN2 / CMIN2) | $49.99/yr | Annual | [Order LA Premium](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74) |

Two things about that second table. The $4/month configuration that used to sit at the bottom of LightLayer's Los Angeles range was retired on September 30, 2026, and the lowest on-sale price moved up to $5/month. LightLayer's notice also said that plans bought before the change keep their configuration and their renewal price. Anyone quoting you $4/month today is working from a page that stopped being true in September.

## Three route tiers, one set of specs

The 1 GB annual plans are the clearest example of how LightLayer prices things. Manila and Taiwan cost $24.99 whichever route you pick. In Los Angeles, the identical box costs $29.99 on Global, $39.99 on Standard and $49.99 on Premium.

Nothing about the CPU, RAM or disk changes between those three. You're paying $20 a year for routing.

- **Global** is the international path. Cheapest, and fine for bots, APIs, cron jobs, staging environments, or anything serving users outside China.
- **Standard** sits in the middle and is the tier to ask about if your traffic is mixed.
- **Premium** is the CN2 / CMIN2-optimized path, positioned for connection quality into mainland China. If your users are there and latency is the reason you're buying, this is the one that addresses it.

Los Angeles also comes in two bandwidth shapes: unmetered at a lower port speed, or a monthly transfer cap at a higher port speed. Pick based on which number you'd rather watch. An unmetered 100 Mbps port won't surprise you with an overage bill, and a metered 200 Mbps port moves more data faster until the cap hits.

Worth saying plainly: "accepts Alipay" and "good for mainland China" are separate claims, and plenty of hosts that take Alipay have no China-optimized routing at all. LightLayer reserves that for the Premium tier, so don't buy Global and expect the same path.

👉 [Compare the Los Angeles Global, Standard and Premium carts](https://account.lightlayer.net/index.php?/cart/los-angeles/&affid=74)

## Paying with Alipay: what shows up on the invoice

Alipay is listed among LightLayer's accepted methods alongside PayPal, credit cards and cryptocurrency. You pick it at the invoice step, confirm in the Alipay app, and the invoice is marked paid. No card, no PayPal balance, no reseller in the middle.

LightLayer's plan listings don't mention an Alipay surcharge. That isn't the same as a guarantee, because this is a real variable in the market. Infrawire adds a disclosed 3% to Alipay invoices and shows it before you confirm; Cloudzy states it charges nothing extra and that Alipay pays the same price as a card. Both are legitimate, and they show why you check the total on the invoice rather than trusting the headline price.

Currency is the other moving part. LightLayer prices in USD, so the RMB amount is whatever Alipay's rate produces on the day. Some hosts bill in euros instead, which adds a second conversion layer if your balance is in RMB.

## What 12 months actually costs

Monthly at the entry price is $60 a year. The Taiwan or Manila annual plan is $24.99 for the same 1 GB of RAM and 50 GB of NVMe, so annual billing saves roughly $35, or about 58%. Even against Cloudzy's promotional $2.48/month for 512 MB, LightLayer's annual works out to about $2.08/month with twice the memory. The catch is that you're paying for a year up front to a host with a narrow refund policy, which the next section covers.

Pay As You Go starts at $5.60/month and is the tier that makes sense when 1 GB is too tight but 32 GB is absurd. You set the core count and RAM yourself instead of picking a fixed size, so a 2-core / 2 GB build lands well under the Business price. Business at $53.60/month is for people who genuinely need 32 cores on a Premium route; a hobby blog or a single Docker stack never gets near it.

On renewal: LightLayer's September lineup notice said existing plans keep their renewal pricing through the change, and third-party write-ups of their promotions describe renewal rates holding rather than doubling. Verify the renewal figure for whatever you buy at checkout anyway, since promotional pricing on new orders can move.

👉 [Take the $24.99/year Taiwan plan](https://account.lightlayer.net/index.php?/cart/taiwan/&affid=74)

## Refunds at LightLayer: provider fault only

This is the part to read before you pay for a year.

LightLayer's refund policy covers provider-attributable faults only. Regular-priced products and promotional products aren't refundable for reasons that aren't LightLayer's, which includes you deciding the route isn't fast enough or the plan is too small. Compare that with Cloudzy's 14-day money-back window, Infrawire's 7 days, or RackNerd, which has no standard guarantee either.

That single policy changes the sensible buying order. If you already know the Global route is fine for your workload, the $24.99 annual plan is the cheapest way in and the refund question never comes up. If you're buying for latency and haven't tested the path yet, spend $5 on one month first and measure it. Five dollars is cheap insurance against a $49.99 annual plan you can't return.

👉 [Test it on a $5 monthly plan before committing to a year](https://account.lightlayer.net/?affid=74)

## Locations and who each one suits

LightLayer runs data centers in Hong Kong, Taiwan, Japan, Thailand, Singapore, the Philippines, the United States, the United Kingdom and Germany. For anyone paying in RMB, the Asian footprint is the reason to look at this brand at all: Hong Kong, Taiwan and Japan cover most latency-sensitive use cases without crossing the Pacific.

Two caveats on the location list. Not every location necessarily offers all three route tiers at every plan size, so confirm your pick inside the cart rather than assuming. And the Asian locations aren't automatically China-optimized; that's the Premium tier's job, and it's priced accordingly.

## When a different host fits better

LightLayer's weak spot is the refund policy, and its second weak spot is that it's a young brand under Megalayer with a large but partly new location list. If either matters more than price, these are the verified alternatives.

| Provider | Entry price | Entry spec | Billing | Alipay surcharge |
| --- | --- | --- | --- | --- |
| LightLayer | $5.00/mo · $24.99/yr | 1 vCPU · 1 GB · 50 GB NVMe | Monthly or annual | Not stated |
| Cloudzy | $2.48/mo | 1 vCPU · 512 MB · 20 GB NVMe | Hourly, monthly, yearly | None |
| LightNode | $7.71/mo | 1 vCPU · 2 GB · 50 GB NVMe | Hourly | Not stated |
| Infrawire | €8.30/mo | 2 cores · 4 GB · 40 GB NVMe | Monthly | 3%, shown before payment |
| RackNerd | $11.29/yr | 1 core · 1 GB · 24 GB SSD | Annual | Not stated |

Cloudzy's $2.48 and Infrawire's €8.30 are both 50%-off promotional rates against list prices of $4.95 and €16.60, and neither page states what renewal costs. Cloudzy gives 14 days to change your mind and refunds to the original payment method; Infrawire gives 7. RackNerd's annual pricing is the cheapest per gigabyte of the group but comes with no standard refund guarantee, and its Asia-optimized Los Angeles DC-02 location is limited to the 2 GB tier and above, stock permitting.

Three situations where you should look elsewhere first:

- **You want hourly billing to test a dozen locations.** LightNode bills hourly across 40+ locations from $7.71/month, which is a better fit for shopping around than an annual commitment.
- **You need a Windows remote desktop.** A Windows-RDP specialist like rdp.monster starts at $8.99/month for 2 dedicated cores and 6 GB, and states outright that it has no China-optimized routes.
- **You need an exit window.** Cloudzy's 14 days and Infrawire's 7 days both beat a provider-fault-only policy if you're unsure the host will work out.

## Which vps with alipay payment to buy, by situation

- **One small box for a bot, a proxy, a VPN endpoint, or a staging site, and location doesn't matter:** Taiwan or Manila annual, $24.99/year. About $2.08/month for 1 GB and 50 GB of NVMe is hard to argue with.
- **Users in mainland China where latency drives the decision:** Los Angeles Premium at $49.99/year, or check whether Hong Kong or Taiwan offers the Premium route at your plan size inside the cart.
- **You need more than 1 GB but less than 8:** Pay As You Go from $5.60/month, built to your own core and RAM count.
- **You're not sure the network suits you yet:** one month at $5 first. The refund policy is the reason.

Three things to confirm before you enter your Alipay password: the invoice total after Alipay is selected, since that's where any surcharge would appear; the renewal price of the promotional rate you're buying; and whether your chosen location offers the route tier you actually want.

👉 [Open LightLayer's plan list and check the Alipay total before you confirm](https://account.lightlayer.net/?affid=74)
