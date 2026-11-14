> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · Kaspa Testnet-10 only. tKAS has no value.

# Lock (pre-run 44)

Locked before the first submit.

- Network: Testnet-10. The desk node is not restarted and it is not stopped.
- One knob: the fee cap, 6,000 to 12,000 tKAS. The rate stays 920 sompi per gram. One hundred chains stay. The ready cap stays off. No second lane. No payment ladder.
- The lane submits only to the desk node. While it is on, it slows other users' low-fee transactions on our node.
- The join is setup, named before any submit. At 2026-11-14T18:49:41Z the payment pile had 280 coins at or above 10 tKAS, together 5,019 tKAS, and 2,584 coins between 2 and 10 tKAS, together 17,540 tKAS. After this plan is on origin, and before the lane process, those 2–10 tKAS coins are joined into coins of 40 tKAS on the same pile, up to 120 of them. Coins already at or above 10 tKAS are not spent in the join. Value is not moved onto the funding key.
- No covenant families, no mint line, no guest. The funding key was at 17,905 usable tKAS at 2026-11-14T18:49:41Z, under the 18,000 line. Pre-runs 36 through 43 did not spend it.
- The two keys this series leaves unused stay unused. The lane spends the payment pile.
- One counter: the desk node. The Mini is not reachable. No Mini-armed file.
- Fee cap 12,000 tKAS, moved cap 14,000 tKAS, pile floor 200 tKAS. The lane's existing pause, at mempool size 90,000 or ready mass over 80 blocks, stays. The moved cap sits above the fee cap so it is not the knob.
- Disk line: abort if the desk is under 150 GB free. It was 327.25 GB after pre-run 43.
- A miss is a retry with the fix written first. This page is not rewritten to match the result.
