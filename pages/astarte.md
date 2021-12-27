---
layout: default
---

# Astarte Testnet Debrief

![A poem about astarte, by block pane](https://raw.githubusercontent.com/envoylabs/blog/gh-pages/assets/astarte.png)

Most people will know that Juno maintains a long-running testnet called `uni` for testing smart contracts and mainnet upgrades.

However, in order to not disrupt testing of smart contracts on `uni` in the run-up to the Moneta release, it became necessary to spin up a series of short-lived `astarte` testnets. We took on the responsibility of co-ordinating these, while we continued to work behind-the-scenes on the upgrade itself.

These four testnets in about three weeks represented a huge amount of effort on the part of the Juno validators that participated.

In one case, the window for submitting gentxs before coining a genesis file was only an hour-and-a-half. If you were in Europe, the window was after midnight.

Bugs were found, heads were banged against tables, and eventually, Moneta was released.

The validators who participated, according to the dumps we took from our node peers (and the gentx records) were:

|Validator Moniker | Testnets participated |
| ---------------- | --------------------- |
| block pane       | 4                     |
| SpacePotato      | 4                     |
| polkachu         | 4                     |
| disperze         | 4                     |
| SkyNet           | 3                     |
| RHINO            | 3                     |
| ben2x4           | 2                     |
| meow             | 2                     |
| Messi            | 2                     |
| HighlanderNodes  | 2                     |
| Mercury          | 2                     |
| jabbey           | 1                     |
| Komikuri         | 1                     |

The bracketed figure is how many testnets were participated in. If we've got the number wrong, then shout at us on discord and we will amend. Some of validators we've got down as 2 probably participated in 3/4, but heck, we're tired.

Obviously _thank you_ to all the validators that participated in these testnets. Without the Astarte team, neither Moneta nor the security patch could have been released on the demanding timescale we had.

People worked over Hannukah, and in the run-up to Christmas, sometimes late at night or early in the morning, sacrificing time with family and loved ones.

After the Moneta release, within one hour, the `astarte-3` team upgraded to a security patch, and helped verify it so that it could be rolled out to validators to patch before the Christmas holiday. In particular, special thanks go to `SkyNet`, `jabbey`, `RHINO`, `Disperze`, `mercury` `SpacePotato`, `Messi` and `Polkachu` for jumping on the upgrade and testing immediately.

A **special special** thanks goes to `[ block pane ]` who helped coordinate and sense check that upgrade between two canary nodes (`needlecast` and `[ block pane ]`), before it was rolled out to `astarte-3`.

It goes without saying that these validators deserve the support of the community, not just for the cost of the servers they were running (for those that did all four nets, for a month) but also for the blood, sweat, tears, and sometimes memes that they shed to get Moneta and the security patch out the door.

Thank you all 🙏
