# WYNN: losses of every buyer

Generated 2026-11-03T00:28:20 UTC from the trade table behind the main report (every buy and sell on the bonding curve and the PumpSwap pool). Net loss per wallet = SOL paid in buys - SOL received in sells - value of any remaining tokens at today's pool price (4.582e-08 SOL/WYNN). USD at trade time uses the hourly SOL/USD close; today's SOL/USD = 93.62. Full per-wallet table: `exhibits/buyer_losses.csv`.

## Aggregate

| Group | Wallets | SOL paid | SOL received | Holdings now (SOL) | Net loss (SOL) | Net loss (USD at trade) | Median loss (SOL) |
|---|---|---|---|---|---|---|---|
| All buyers other than the creator and the cohort | 6470 | 16,211.0 | 15,928.5 | 5.7 | 2,319.8 | 176,425.9 | 0.001 |
| ... of which net losers (loss > 0.01 SOL) | 2659 | 7,867.5 | 5,545.5 | 5.4 | 2,316.6 | 176,178.3 | 0.114 |
| ... net losers that never transferred tokens out (conservative count) | 2485 | 7,196.8 | 5,189.9 | 5.3 | 2,001.6 | 152,333.5 | 0.107 |
| ... net losers whose first buy came after the post of 2026-06-30 16:42 | 2397 | 6,834.9 | 4,676.4 | 5.3 | 2,153.1 | 163,751.9 | 0.112 |


The 35 cohort wallets paid 155.5 SOL and took out 610.0 SOL, a net gain of 454.5 SOL. The creator wallet itself paid 274.5 SOL (238 SOL of it in seven pool buys between 2026-06-30 and 07-06, before the cohort's sells of 07-13), received 13.2 SOL and burned 180.2M tokens, so on its own it shows 261.3 SOL out of pocket; the group's net gain sits in the cohort wallets. 1897 other wallets also came out ahead, by 2,041.0 SOL in total (wallets that sold early). The rest is the loss of the 2659 wallets above.

## Loss distribution (net losers other than the creator and the cohort)

| Net loss | Wallets | Total SOL | Total USD at trade |
|---|---|---|---|
| 0.01 to 0.1 SOL | 1249 | 50.6 | 3,836 |
| 0.1 to 1 SOL | 1039 | 352.4 | 26,618 |
| 1 to 10 SOL | 335 | 946.1 | 71,875 |
| 10 to 100 SOL | 35 | 749.4 | 57,973 |
| over 100 SOL | 1 | 218.2 | 15,876 |


## By day of first purchase

| First buy (UTC) | Wallets | SOL paid | Net loss (SOL) | Net loss (USD at trade) |
|---|---|---|---|---|
| 2026-06-30 | 887 | 3,494.2 | 898.0 | 65,971 |
| 2026-07-01 | 840 | 2,405.1 | 747.5 | 55,751 |
| 2026-07-02 | 168 | 454.3 | 119.2 | 9,500 |
| 2026-07-03 | 77 | 195.6 | 54.7 | 4,508 |
| 2026-07-04 | 107 | 192.5 | 71.8 | 5,990 |
| 2026-07-05 | 221 | 415.8 | 140.7 | 11,486 |
| 2026-07-06 | 53 | 107.2 | 26.3 | 2,159 |
| 2026-07-07 | 60 | 228.0 | 100.3 | 8,440 |
| 2026-07-08 | 27 | 24.0 | 17.3 | 1,349 |
| 2026-07-09 | 36 | 64.3 | 15.2 | 1,183 |
| 2026-07-10 | 31 | 57.6 | 30.1 | 2,388 |
| 2026-07-11 | 15 | 21.2 | 5.6 | 405 |
| 2026-07-12 | 75 | 128.8 | 69.8 | 5,397 |
| 2026-07-13 | 51 | 74.4 | 18.3 | 1,563 |
| 2026-07-14 | 4 | 1.9 | 0.8 | 59 |
| 2026-07-16 | 1 | 0.0 | 0.0 | 1 |
| 2026-07-18 | 2 | 1.2 | 0.2 | 15 |
| 2026-07-19 | 1 | 0.1 | 0.1 | 11 |
| 2026-07-21 | 1 | 0.0 | 0.0 | 0 |
| 2026-07-23 | 1 | 0.0 | 0.0 | 1 |
| 2026-08-23 | 1 | 1.1 | 0.6 | 0 |


## Largest 50 losses

| Wallet | First buy | Buys | SOL paid | Sells | SOL received | WYNN held now | Net loss (SOL) | USD at trade | Sent tokens out |
|---|---|---|---|---|---|---|---|---|---|
| [`9bMWuK…TsMW`](https://solscan.io/account/9bMWuKKGhANBDvhPcs9sf31V6pEXC4JoKRVcKqB5TsMW) | 2026-06-30 17:29:20 UTC | 8 | 320.04 | 2 | 101.84 | 0 | 218.20 | 15,876 |  |
| [`CHvxnJ…j532`](https://solscan.io/account/CHvxnJQm4wjzUaUsLmX7CXeWRxUZ4djyCwPNxwAXj532) | 2026-07-01 03:01:26 UTC | 18 | 101.43 | 1 | 8.12 | 45,195,813 | 91.24 | 7,250 |  |
| [`6eQH9P…g6i5`](https://solscan.io/account/6eQH9PcE8H5f6WWQD3Qfoqwwmp22CkLVpHVVcpSVg6i5) | 2026-07-01 08:32:43 UTC | 1 | 62.67 | 1 | 0.49 | 0 | 62.18 | 4,717 | yes |
| [`CtH9NC…mtk6`](https://solscan.io/account/CtH9NCLECxoJSzFG4QvYq7gLzGAuXnKSw7aXpt43mtk6) | 2026-07-01 08:29:00 UTC | 23 | 140.23 | 3 | 85.80 | 0 | 54.43 | 3,911 |  |
| [`HFyo7q…mJgU`](https://solscan.io/account/HFyo7qUTFTWHphb2V1Us3sQ8gXrTbqurLm6gPZ4QmJgU) | 2026-06-30 18:12:34 UTC | 9 | 39.49 | 2 | 5.26 | 0 | 34.23 | 2,624 |  |
| [`GqnPwD…eS89`](https://solscan.io/account/GqnPwDpi9JThzfyk7JvUihuX2pcS5VkTb1PX2Br2eS89) | 2026-06-30 18:56:08 UTC | 14 | 49.46 | 11 | 21.79 | 0 | 27.68 | 2,076 |  |
| [`8WWWmb…u2rh`](https://solscan.io/account/8WWWmb5Jggo7V7exqLny88RRBNchqTJbzh29EsMJu2rh) | 2026-07-01 01:13:52 UTC | 5 | 46.92 | 1 | 21.19 | 0 | 25.73 | 2,031 |  |
| [`mP4tnN…ayQP`](https://solscan.io/account/mP4tnNkwAtRLpSZG5CqcH3CVPJHgVw7XH3j6YRyayQP) | 2026-06-30 16:39:52 UTC | 91 | 111.14 | 53 | 86.11 | 20,630 | 25.03 | 2,172 |  |
| [`FBnWJd…qzcD`](https://solscan.io/account/FBnWJdRwjupDPjAH5JN7rTi9P9CrnSx1i17RsinpqzcD) | 2026-07-01 08:29:59 UTC | 3 | 48.64 | 1 | 24.93 | 0 | 23.71 | 1,784 |  |
| [`AeuLW8…aXiN`](https://solscan.io/account/AeuLW8uUqdxBEKGTdyNHLqRt8Wr4Mem1o2Bhxt1kaXiN) | 2026-07-04 17:36:34 UTC | 113 | 24.42 | 1 | 0.74 | 0 | 23.68 | 1,991 |  |
| [`HLyCG9…p9GE`](https://solscan.io/account/HLyCG98sJ8cDECGMcqLRnUKi2WxdgtDJXaqwdv2Kp9GE) | 2026-07-12 21:03:26 UTC | 3 | 39.13 | 1 | 16.28 | 0 | 22.86 | 1,750 |  |
| [`9vJPXX…yN7N`](https://solscan.io/account/9vJPXXhM1411zkdNhpM4UpMcdqqFp3qL9RjJxNHxyN7N) | 2026-07-07 16:05:01 UTC | 2 | 22.23 | 1 | 1.89 | 0 | 20.34 | 1,689 |  |
| [`ASLjDS…RFq9`](https://solscan.io/account/ASLjDS6R8V4YUva5gTjRP2mttkkh5iF98te6p47SRFq9) | 2026-06-30 18:25:45 UTC | 15 | 19.84 | 1 | 0.24 | 0 | 19.60 | 1,456 |  |
| [`DJ8toq…Fvng`](https://solscan.io/account/DJ8toqg4vB5re8wDBx4svpfA9oFxamGLyeRcymJZFvng) | 2026-07-01 08:18:02 UTC | 18 | 37.82 | 5 | 18.39 | 0 | 19.43 | 1,493 |  |
| [`29Y2wZ…HPa5`](https://solscan.io/account/29Y2wZstBBCSb9ZpdE42Y1bnTae6iitRXqCPH5fzHPa5) | 2026-07-03 18:36:46 UTC | 1 | 20.81 | 1 | 1.94 | 0 | 18.88 | 1,562 |  |
| [`FtiD7o…Ntx5`](https://solscan.io/account/FtiD7oFS8QkYNSNsEMqjXLFozxAbBuG4yPsmdrH1Ntx5) | 2026-06-30 18:08:50 UTC | 6 | 45.91 | 4 | 27.43 | 0 | 18.48 | 1,183 |  |
| [`6cmrPn…QThv`](https://solscan.io/account/6cmrPnco8aQYpMD7YLnjsFFi4V3kxK3VQMqwvNFRQThv) | 2026-07-02 10:38:09 UTC | 4 | 18.00 | 1 | 1.89 | 0 | 16.11 | 1,326 |  |
| [`GZX9US…Hhbr`](https://solscan.io/account/GZX9USGjrRm82QihsLVte73nhLB1Qnizvury75SCHhbr) | 2026-07-01 08:36:46 UTC | 5 | 25.34 | 1 | 9.37 | 0 | 15.97 | 1,187 |  |
| [`GiEnKV…G4Hz`](https://solscan.io/account/GiEnKVdeaJn8vCMxzDkzNnGNK7WeQSJd5XpYmUT5G4Hz) | 2026-06-30 17:50:49 UTC | 3 | 15.89 | 0 | 0.00 | 0 | 15.89 | 1,181 | yes |
| [`8geKre…yQYx`](https://solscan.io/account/8geKrefuE4hEBaXchivumtLfQ4YJWezdRL8pXnYmyQYx) | 2026-07-01 08:43:49 UTC | 1 | 21.92 | 1 | 6.35 | 0 | 15.57 | 1,159 |  |
| [`3KKT6g…wKjS`](https://solscan.io/account/3KKT6gGf5mvjuMVzRq69FQpYKpR8yNyttETR8twBwKjS) | 2026-07-01 08:46:06 UTC | 12 | 44.12 | 2 | 28.71 | 0 | 15.41 | 1,106 |  |
| [`7gUCbp…Dn5W`](https://solscan.io/account/7gUCbpeRt8W5mp1k4PCQKsgaLEJ5pJAEQcfVXt2rDn5W) | 2026-07-01 08:33:22 UTC | 4 | 38.73 | 3 | 23.38 | 0 | 15.35 | 1,135 |  |
| [`BoeAxs…vYxk`](https://solscan.io/account/BoeAxs9HpUidBrntxn6W1AVwEGMowS69UYwhPThxvYxk) | 2026-07-01 22:41:32 UTC | 4 | 27.73 | 1 | 13.24 | 0 | 14.50 | 1,086 | yes |
| [`3a7zgq…wWT7`](https://solscan.io/account/3a7zgqiCvnmuiha7abXXWvoPrgaKEtL8aNYNTJxSwWT7) | 2026-06-30 19:00:56 UTC | 3 | 13.73 | 0 | 0.00 | 0 | 13.73 | 1,042 | yes |
| [`8WMZzj…HFLJ`](https://solscan.io/account/8WMZzjwwJvdksnBaEK23AWQX59bKi8XFt86novKaHFLJ) | 2026-07-07 20:37:32 UTC | 2 | 35.76 | 1 | 22.41 | 0 | 13.35 | 1,171 |  |
| [`AVJAHC…Vh5x`](https://solscan.io/account/AVJAHC8jqcTNBUcB9d5PibN2TBRGERMKN4Uinj8KVh5x) | 2026-07-01 09:19:14 UTC | 1 | 12.88 | 0 | 0.00 | 0 | 12.88 | 970 | yes |
| [`CJmfp1…TsC2`](https://solscan.io/account/CJmfp1nQSdEQgBmjNg6AAsKzDJ9Q35CBamWirDKuTsC2) | 2026-07-02 17:29:03 UTC | 1 | 12.75 | 1 | 0.24 | 0 | 12.52 | 1,029 |  |
| [`7FVrjA…V7tk`](https://solscan.io/account/7FVrjAR1HYRrgMnJ5RFRaS9io4N97oybnXHxknvMV7tk) | 2026-07-01 14:48:26 UTC | 1 | 12.50 | 0 | 0.00 | 3,648 | 12.50 | 959 | yes |
| [`AzffGg…3FYi`](https://solscan.io/account/AzffGgqDuv3eNmjM9cq4rEcLb9d1Na8uh9nrszFq3FYi) | 2026-06-30 17:00:00 UTC | 4 | 34.71 | 3 | 22.24 | 0 | 12.47 | 913 |  |
| [`EFLdio…azvT`](https://solscan.io/account/EFLdiojyKL3DLLShYGj2WsK6bea5vyeSu9cWQUYWazvT) | 2026-07-08 03:28:52 UTC | 2 | 12.30 | 0 | 0.00 | 1,727,702 | 12.22 | 962 |  |
| [`FVr2ZV…q5gy`](https://solscan.io/account/FVr2ZVdBvhR23x9D5rbDHR8o3mUvGgKaLqxNWN4jq5gy) | 2026-07-05 17:33:56 UTC | 1 | 11.35 | 1 | 0.08 | 0 | 11.28 | 921 |  |
| [`HkBmJG…VDQL`](https://solscan.io/account/HkBmJGm1QpgupaXWxvPtEfHEbxzCiP73qeL8riLcVDQL) | 2026-06-30 16:39:56 UTC | 1 | 13.79 | 1 | 2.83 | 531 | 10.97 | 803 |  |
| [`Fo9qyq…CRmd`](https://solscan.io/account/Fo9qyqex4KiWB38e16fcStCVzVASxJxUKbUwzJWFCRmd) | 2026-07-07 07:58:23 UTC | 4 | 12.27 | 1 | 1.47 | 0 | 10.79 | 955 |  |
| [`8bVKpM…feAn`](https://solscan.io/account/8bVKpMbfso13FGENWnaKNCDfYVrYr4ssCeMU8sg1feAn) | 2026-07-02 10:57:54 UTC | 21 | 36.78 | 8 | 26.56 | 0 | 10.22 | 788 |  |
| [`Eyx5vV…1w8R`](https://solscan.io/account/Eyx5vViadT2MqRUvzSTxV6cNMEeaN8Jttxi8giVC1w8R) | 2026-07-12 10:23:11 UTC | 5 | 16.17 | 1 | 6.04 | 0 | 10.13 | 790 |  |
| [`AAiJtW…B9BQ`](https://solscan.io/account/AAiJtWctsqhbf87Y7X6ru6KSuzKZfWA2uBgoRmpxB9BQ) | 2026-07-07 14:34:42 UTC | 8 | 42.97 | 6 | 32.93 | 0 | 10.04 | 803 | yes |
| [`4TEcKe…sGtk`](https://solscan.io/account/4TEcKeSjmMf4Ecmvp1qMBLZqyj2GfLJaJ14Ckh6YsGtk) | 2026-07-12 17:37:31 UTC | 1 | 9.91 | 0 | 0.00 | 0 | 9.91 | 766 | yes |
| [`HDrDJn…aE8s`](https://solscan.io/account/HDrDJnZEDe87y7fqCnboCgR3B4wx6Sis9NUa1z9naE8s) | 2026-06-30 21:36:10 UTC | 12 | 45.51 | 6 | 35.69 | 0 | 9.82 | 745 |  |
| [`79E6G7…bSyg`](https://solscan.io/account/79E6G7QTigbshJ2qaDvJDx1SGh1EXAYCqvqn1WkFbSyg) | 2026-07-04 18:56:48 UTC | 1 | 9.77 | 1 | 0.11 | 0 | 9.66 | 801 |  |
| [`F8y8mC…93jH`](https://solscan.io/account/F8y8mCfPvc1VyG7uVEkLP9xpi2wobAp6NYptzyAj93jH) | 2026-06-30 17:18:10 UTC | 14 | 84.72 | 5 | 75.16 | 0 | 9.56 | 756 |  |
| [`4UXJUG…T4JM`](https://solscan.io/account/4UXJUGqXRqCHeJJDrSEG9gZyyPnkrDY7s8VXYiK3T4JM) | 2026-07-01 11:51:16 UTC | 2 | 9.42 | 0 | 0.00 | 876,728 | 9.38 | 703 |  |
| [`5gUkkt…geAN`](https://solscan.io/account/5gUkktEnaZ43r6hV1q3BfKwMswYn7L2oxBdW5Zh2geAN) | 2026-07-07 11:49:34 UTC | 13 | 27.79 | 1 | 18.44 | 0 | 9.35 | 825 |  |
| [`HDgvoj…K7yw`](https://solscan.io/account/HDgvojZ63jHRZT3SbkePLVarjybdhbGiTKhbYAh9K7yw) | 2026-07-12 14:54:02 UTC | 1 | 9.18 | 0 | 0.00 | 2,378,223 | 9.07 | 701 |  |
| [`8sjxhm…gUyE`](https://solscan.io/account/8sjxhmQg3AvijGMfXVqakFRXbZv2kUBdxezKyZuugUyE) | 2026-06-30 16:50:10 UTC | 2 | 35.36 | 2 | 26.42 | 0 | 8.94 | 654 |  |
| [`86Z9nb…P88b`](https://solscan.io/account/86Z9nbobKU3kAGHd6wLeofHMiHqvbf3UiyPnunz6P88b) | 2026-06-30 19:10:08 UTC | 3 | 11.49 | 1 | 2.67 | 0 | 8.82 | 645 |  |
| [`8XEoYz…PNoR`](https://solscan.io/account/8XEoYzoFUAfQWCSKw51PLRnU9RqW4xghXsYxbzj9PNoR) | 2026-07-05 14:48:56 UTC | 1 | 8.74 | 0 | 0.00 | 1,103,932 | 8.69 | 706 |  |
| [`2TP9k2…1rSW`](https://solscan.io/account/2TP9k2MrY33tGgYtFHrMMoGuuEFxsLprPtsJBDuR1rSW) | 2026-07-02 02:12:24 UTC | 5 | 9.45 | 1 | 0.95 | 0 | 8.50 | 674 |  |
| [`BM9Ccy…jvMN`](https://solscan.io/account/BM9CcyErJcu2mjrFvUsRRrD3snGeHDDVirJLvL6EjvMN) | 2026-06-30 16:27:08 UTC | 85 | 38.48 | 66 | 30.13 | 29,196 | 8.36 | 615 | yes |
| [`ARfCRF…x2fP`](https://solscan.io/account/ARfCRF98ZADiJgCuGwtXSJoyCBtgwxVvEV5Am8xex2fP) | 2026-07-10 08:49:43 UTC | 2 | 11.21 | 1 | 2.86 | 0 | 8.35 | 674 |  |
| [`EHkUsj…rfE4`](https://solscan.io/account/EHkUsjWX4P56z7RyoV9C6XnZM5x26HQfjKC4p2ierfE4) | 2026-07-06 22:28:29 UTC | 4 | 27.28 | 3 | 19.12 | 0 | 8.15 | 661 | yes |


## Method notes

- A wallet's SOL paid/received is the pool's side of each trade (what left or entered the pool), so routing fees and priority fees are not included; the wallet's own cost is slightly higher.
- 'USD at trade' converts each trade at the SOL/USD hourly close of that hour; it is the dollar value at the time, not today's.
- Remaining holdings are valued at today's pool price. Selling them would move the price further down, so this understates the loss of anyone still holding.
- A wallet that transferred tokens to another wallet may have sold them from there; such wallets are flagged ('Sent tokens out') and excluded from the conservative count.
- 'Net losers whose first buy came after the post of 2026-06-30 16:42' uses the post time decoded from its id (section 3 of the main report).
- Wallets are not people: one person may hold several wallets, and some losers are bots. The counts are of addresses.
