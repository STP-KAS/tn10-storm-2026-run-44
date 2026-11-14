> **Experimental. We are just trying this.** [Disclaimer](../DISCLAIMER.md) · This page does not start a machine. Pre-run 44. Not Wednesday. Not Tuesday. Not pre-run 1 to 43.

# Targets

Pre-run 43 held one hundred chains with the ready cap off, rate 920, and a fee cap of 6,000 tKAS. Pending reached 100. Submit-OK was 449–661 a minute. In the twelve samples while our heavy class was 88–99, the template's heavy count stayed 1, and ready mass was 54.01–80.24 blocks. The priority fee estimate on those samples was 1,490.92–1,597. The lane wrote a hold at 18:41:13Z on ready mass 80.24 and a clear at 18:41:33Z, when the probe's sample was empty. It did not trip a second time. The fee cap stopped new submits at 18:43:16Z, fees 6,012.63 tKAS. The rate is already the knob we just turned. The next single knob is the fee cap, 6,000 to 12,000 tKAS, so the six minutes are not cut by the same budget.

**Question.** On our desk node, with one hundred chains, the rate held at 920, and no ready cap, what happens to ready mass and to the lane's pause when the fee cap is 12,000 tKAS instead of 6,000? We do not expect the template's heavy count of this shape to rise. Finding 33 already says a second transaction of about 267,000 storage mass does not fit a 500,000-mass block.

**Target.** The lane runs only in the middle step and is at zero at the end. A table, written after the tail from this run's own files, shows template storage mass, template transaction count, ready mass, and the fee estimate, for the baseline minutes, the hold minutes, and the return minutes. **Met means the table exists and the lane is at zero, not that a particular theory won.** If the fee cap or the pause stops new submits before the six minutes are up, the table still counts. At about 600 submits a minute and about 2.453 tKAS each, six minutes is about 8,800 tKAS, under 12,000. The cap may still end the hold. That is accepted. The cap's new level is the knob. A second rate change is not.

## Why the twelve families are not in this run

At 2026-11-14T18:49:41Z the funding key's usable balance (coins over 3 tKAS, above that line) was 17,905 tKAS. That is the same figure as the 18:31:03Z read. Pre-runs 36 through 43 did not spend that key. A family window aborts under 18,000 tKAS. This run does not start the families, the mint line, or the guest. The two keys this series leaves unused stay unused.

## The pile, read before the arm

The lane takes a coin only when that coin is at or above 10 tKAS. At 2026-11-14T18:49:41Z the payment pile had 280 such coins, together 5,019 tKAS, and 2,584 coins between 2 and 10 tKAS, together 17,540 tKAS. 5,019 tKAS does not cover a 12,000 tKAS fee cap.

After this plan is on origin, and before the lane process starts, this run joins the pile's own coins that are between 2 and 10 tKAS into coins of 40 tKAS on the same pile, and stops at 120 of those coins or sooner if a submit is rejected. It does not spend a coin already at or above 10 tKAS. It does not touch the funding key or the two unused keys. Value stays on the pile. Nothing moves onto the funding key. The lane starts only after a fresh read can see the new coins.

## The one change, written before the arm

**Fee cap 12,000 tKAS. The rate stays 920 sompi per gram. One hundred chains stay. The ready cap stays off.** Our heavy lane (the same shape as pre-run 43: one input, two outputs, storage mass about 266,666, submitted only to the desk's private node). No second lane. No climb past 920. The moved cap is 14,000 tKAS, so it sits above the fee cap and is not the knob. The pile floor stays 200 tKAS. The lane's existing pause, at mempool size 90,000 or ready mass over 80 blocks, stays in the code. Whether ready mass crosses 80 again, and whether a hold lasts, is what this run is here to observe. That pause is not a second knob. The join above is setup. It is not the knob.

**While it runs it slows other users' low-fee transactions on our node. We say so here, in public.**

| Order | Step | Lane | Length |
|---:|---|---|---:|
| 1 | BASE | off (N=0, ready cap 0) | 3 whole minutes |
| 2 | HOLD | N=100, ready cap off, rate 920, fee cap 12,000 tKAS | 6 whole minutes |
| 3 | RETURN | off | 3 whole minutes |

The desk node is not restarted. One counter: the desk. The Mini is not reachable. No payment flood. No heavy submit to a public node.

Disk line: abort if the desk is under 150 GB free.
