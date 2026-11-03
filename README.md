# WYNN contract: on-chain record

A public record of the Solana token **WYNN** ("The White Bull"), mint
`9E2Q4KKxLS5Y4bu6RKvjg5wQ2kzaLkiVsMt7zwMZpump`, from its creation on pump.fun on
2026-06-30 to 2026-11-01: every trade on the bonding curve and on the PumpSwap
pool, the pool's reserves after each trade, who held what and when, how the
largest early wallets were funded and where their proceeds went, the net
result of every wallet that bought, and the public X posts of the account that
posted the contract address.

Everything here is reconstructed from the public Solana ledger. Every figure in
the report links to the transaction on solscan.io so that it can be checked
without trusting this repository. The record states what the ledger shows and
quotes public posts verbatim. It draws no conclusion about who controlled which
wallet or why; those are questions for the exchanges' records and for the
authorities that can obtain them.

Where the record says "before" or "after the peak", the reference point is the
transaction after which the pool held the most SOL it ever held
(2026-07-01 08:34:19 UTC, 578.96 SOL). It is read off the ledger, not chosen.

## Contents

| File | What it is |
|---|---|
| `WYNN_onchain_record.md` | The report: token facts, the account's posts of the address set against the ledger, the launch and the 35 largest early wallets, holder concentration at the peak, the sells after the peak and the sells of July 2026, funding traces, method and limitations |
| `buyer_losses.md` | Net result of every wallet that ever traded the token: aggregate, distribution, by day, largest 50 |
| `x_posts.md` | The X account's posts from April to October 2026: coverage check, every post mentioning the token, posts matched to the creator wallet's transactions, links |
| `verification.md` | 26 key transactions re-read from an independent RPC node and compared field by field |
| `fig_pool_reserves.png` | SOL held by the pool and the pool price over time |
| `fig_top_sellers.png` | SOL taken out of the pool after the peak, top 15 wallets |
| `screenshots/` | Solscan's public labels for the two exchange wallets; the post of 2026-06-30 16:42 UTC |
| `exhibits/swaps.csv` | Every trade: time, slot, signature, wallet, side, tokens, SOL, price |
| `exhibits/pool_reserves_timeseries.csv` | Pool SOL, WYNN and price after every pool trade |
| `exhibits/holders_at_peak_top200.csv` | Holder table at 2026-07-01 08:34:19 UTC |
| `exhibits/all_sells_after_peak.csv`, `sellers_after_peak.csv`, `hourly_sells_after_peak.csv` | Every sell after that moment, by transaction, by wallet, by hour |
| `exhibits/cohort.csv`, `exhibits/cohort_sell_windows.csv` | The 35 wallets that each held at least 5M WYNN at migration, and their sell windows |
| `exhibits/wallet_funding.csv`, `exhibits/wallet_outflows.csv`, `exhibits/clusters.csv` | First funding of the traced wallets, SOL leaving them, groups linked by funder or destination |
| `exhibits/burns.csv` | Every burn |
| `exhibits/buyer_losses.csv` | One row per wallet that ever traded, with SOL paid, received, held and net result |
| `exhibits/x_posts/` | Two browser exports of the X account's timeline, as saved, untouched |
| `exhibits/x_posts_merged.csv`, `exhibits/x_posts_links.csv` | The exports merged and de-duplicated; every link posted |
| `exhibits/x_posts_oembed.jsonl` | The text of every post as served by X's public embed endpoint, with fetch time |
| `exhibits/tweet_2071997912545120318_oembed.json` | The same for the post of 2026-06-30 16:42 UTC |

## How it was built

1. Every transaction signature touching the mint or the pool was listed from
   the ledger (71,636 successful transactions), in exact block order.
2. Each transaction was parsed, and for each wallet the change in WYNN and SOL
   was taken from the validator-recorded pre- and post-balances, not from any
   parser's interpretation.
3. A trade is a transaction in which the pool's (or, before migration, the
   bonding curve's) WYNN balance changes; the counter-party is the wallet whose
   WYNN moved the other way; price is the pool's SOL change over its WYNN change.
4. Cumulating the pool's changes reproduces the pool's live vault balances to
   the lamport, which shows no pool transaction is missing. The peak of that
   series is the reference point for the before/after tables.
5. Holder tables are cumulative sums per wallet up to a slot. Funding traces
   follow each wallet's first incoming SOL to its sender, and SOL leaving each
   wallet to its destination, with token accounts and program accounts
   resolved so that only wallet-to-wallet movements are counted.
6. Key transactions were re-read from a second, independent node and compared.
7. The X posts were captured in a logged-in browser from the account's profile
   and its "Posts & replies" tab, then each post's text was fetched again by id
   from X's public embed endpoint. Posting times are decoded from the post ids,
   which encode creation time to the millisecond; they agreed with the
   displayed timestamps in every case.
8. Exchange names for two funding wallets are Solscan's public labels as shown
   in a browser on 2026-11-01 (screenshots included); they are an explorer's
   attribution, not a ledger fact.

Dollar figures use the hourly SOL/USD price at the time of each trade. Wallets
are addresses, not people; one person may hold several, and some are automated.

## Checking it

Every figure here comes from the public Solana ledger and links to the
transaction it is taken from. Any of them can be checked by opening the link,
or by reading the same transaction from any Solana node. The method is
described in full in the last section of `WYNN_onchain_record.md`.

## Corrections

If any figure here does not match the ledger, open an issue citing the
transaction signature. The record will be corrected and the correction noted.
