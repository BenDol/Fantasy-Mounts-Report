# Fantasy Mounts: bug reports

This is where you report bugs in [Fantasy Mounts](https://fantasymounts.com), the Minecraft mod of fantasy mounts to
find, tame, breed and ride, on Forge, NeoForge, Fabric and Quilt.

**[Report a bug](https://github.com/BenDol/Fantasy-Mounts-Report/issues/new/choose)** ·
[Search existing reports](https://github.com/BenDol/Fantasy-Mounts-Report/issues?q=is%3Aissue)

No GitHub account? Use **Report a bug** on [fantasymounts.com](https://fantasymounts.com): the site posts your report
here for you, labelled `via: website`.

## Bugs only

This tracker takes **bug reports only**. Suggestions, ideas and feature requests opened here are closed.

Have an idea for a mount, an ability or a change? Become a **Trailblazer** on
[Patreon](https://patreon.com/fantasymounts) and share it with the developer in the Trailblazer channels on our
[Discord](https://discord.gg/HkHPV6Z4zy). Trailblazers also play each month's new mounts before anyone else.

| You have... | Go to |
| --- | --- |
| A bug, a crash, something that looks or works wrong | [Report a bug](https://github.com/BenDol/Fantasy-Mounts-Report/issues/new/choose) |
| A suggestion or an idea | [Become a Trailblazer](https://patreon.com/fantasymounts), then share it on [Discord](https://discord.gg/HkHPV6Z4zy) |
| A question, or trouble installing | `#help` on [Discord](https://discord.gg/HkHPV6Z4zy) |
| A bug in an early-access build | `#beta-feedback` on [Discord](https://discord.gg/HkHPV6Z4zy) |
| An exploit (duplicating items, taking another player's mount, crashing a server on purpose) | [Report it privately](https://github.com/BenDol/Fantasy-Mounts-Report/security/advisories/new), never in a public issue |

## A good report

- **One bug per report**, with a title that says what goes wrong ("Unicorn sinks when ridden into water", not "bug").
- **Steps to make it happen again**, starting from loading the world.
- **A log for every crash**: upload `logs/latest.log`, or the newest file in `crash-reports/`, to
  [mclo.gs](https://mclo.gs) and paste the link. On a server, include the server's log too.
- **Try it with only Fantasy Mounts installed** (plus Fabric API or QFAPI and Forge Config API Port on Fabric and
  Quilt). If the bug goes away, say which other mod brings it back.

## Labels

Your answers in the form label the report for you: the **mod loader** (`loader: ...`), the **Minecraft version**
(`mc: ...`) and the **kind of problem** (`type: ...`). The developer sets everything else.

| Label | Meaning |
| --- | --- |
| `severity: critical` | A crash, a broken world or save, lost mounts or items, a server that won't start, or an exploit |
| `severity: high` | Something important is broken for many players, with no way around it |
| `severity: medium` | Broken, but there is a way around it, or it only happens in some setups |
| `severity: low` | Cosmetic, or a small annoyance |
| `status: needs triage` | New: not looked at yet |
| `status: needs info` | Waiting for the reporter: a log, steps or versions |
| `status: confirmed` | The developer can make it happen |
| `status: cannot reproduce` | The developer couldn't make it happen with the steps given |
| `status: in progress` | Being fixed |
| `status: fixed` | Fixed; the fix ships in the next release |
| `resolution: duplicate` | Already reported; follow the linked report |
| `resolution: not a bug` | Works as intended |
| `resolution: upstream` | Caused by another mod, the loader or Minecraft; report it there |
| `resolution: suggestion` | An idea, not a bug: closed with a pointer to Patreon and Discord |
| `resolution: invalid` | Not about Fantasy Mounts, or not enough to act on |
| `resolution: won't fix` | Won't be changed |
| `via: website` | Sent from fantasymounts.com by a player without a GitHub account; they can't reply here, but may leave a Discord name |

## Maintaining

- **A new Minecraft version or loader:** add it to the form (`.github/ISSUE_TEMPLATE/bug_report.yml`) and create its
  label with the same name, for example `gh label create "mc: 26.4" --color 5c8a3a -R BenDol/Fantasy-Mounts-Report`.
  The website's dialog offers the versions of every published release by itself, so only the label and this form
  need adding.
  The labeller only applies labels that exist, and warns in the Actions log when an answer has none.
- **A new kind of problem:** the label is `type: ` plus the option's words before its colon, in lower case.
- **Severity** is never in the form, and reporters can't add labels themselves, so severity and status are the
  developer's alone.
