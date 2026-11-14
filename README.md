> **Experimental. We are just trying this.** [Disclaimer](DISCLAIMER.md) · Kaspa Testnet-10 only; tKAS has no value.
>
> **This is a pre-run. Pre-run 44.** It is not the Wednesday run. It is not the Tuesday run. It is not pre-run 1 to 43, and it does not edit their repos. A read does not start a runner.

# tn10-storm-2026-11-11-prerun-44

**Pre-run 44: one heavy lane of ours, one hundred chains, no ready cap, fee cap 12,000 tKAS, rate 920 sompi per gram, on the desk node, with the lane off at both ends.** The neuron stays [tn10-storm-2026-11-11](https://github.com/STP-KAS/tn10-storm-2026-11-11). This repo does not edit that repo.

> **Our own testing.** This is our own Kaspa Testnet-10 testing, run on our own machines and nodes. What these pages report is what we observed in this run; it is not a claim of how TN10 or Kaspa behave in general.

| Field | Value |
|---|---|
| Target | A table of the desk template and the desk fee estimate with our lane off, then at one hundred chains and no ready cap at 920 sompi per gram under a 12,000 tKAS fee cap, then off again. The lane returns to zero |
| The change | One knob: the fee cap, 6,000 to 12,000 tKAS. The rate stays 920 sompi per gram. One hundred chains stay. The ready cap stays off. No payment ladder. No second lane |
| Met or not met | **met** on the table and on the lane returning to zero. BASE 18:57–18:59Z: fee estimate 100 / 100 / 100, lane submit 0. HOLD: the lane log shows pending 100, 100, 99, 100, 100 and 100, and submit-OK 652, 541, 450, 603, 568 and 460. In the sixteen samples from 19:00:09Z through 19:05:53Z while our heavy class was present, the template's heavy count is 1, template storage mass 266,682–268,550, our heavy class 87–99 at fee rate 920, and 506–6,951 other transactions sit in the 101–149 fee band. Ready mass in those samples is 54.83–84.9 blocks. The lane's pause tripped at 19:02:31Z on ready mass 84.9 and cleared at 19:02:51Z, then again at 19:05:13Z on ready mass 82.82 and cleared at 19:05:33Z. The fee cap of 12,000 tKAS did not trip. RETURN fee estimate 100 / 100 / 100, pending 0 from 19:06. 3,274 submit-OK, 0 rejects, fees 8,041.95 tKAS |
| Retry count | 0. The next attempt is a new repo. This one is not resumed |
| Core tags | — |
| Status | done. Closed from the lane log and the probe |

Plan, lock, and the prediction are in [plan/PLAN.md](plan/PLAN.md), [locks/LOCKED.md](locks/LOCKED.md), and [plan/PREDICTIONS.md](plan/PREDICTIONS.md). Written before any submit.

While the lane is on, it slows other users' low-fee transactions on our node. We say so here.
