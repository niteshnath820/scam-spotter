# Scam Spotter

Paste a suspicious message. See the warning signs, the risk level and what to do next.

Built for **SETU: Bridge the Gap. Build the Fix** (Forge Realm), Problem Statement **PS-01: Scam Spotter**.

**Live demo:** https://niteshnath820.github.io/scam-spotter/

## What it does

Students and families often get messages that pretend to come from a bank, college or delivery service. Scam Spotter checks a pasted message with clear, visible rules (not only an AI yes/no) and shows:

- each warning sign **highlighted inside the original message**
- a **risk level**: Low, Medium or High, with a score out of 100
- a **plain-language explanation** for every finding
- **safe next steps**, including where to report scams in India (cybercrime.gov.in or 1930)

Your message is checked on your own device. Nothing is sent or stored.

## How the scoring works

Each kind of warning sign counts once. Points are shown next to the exact words that caused them.

| Warning sign | Points |
|---|---|
| OTP / password request (critical) | 40 |
| Lookalike link, e.g. a bank name in a non-official domain (critical) | 25 |
| Suspicious link (critical) | 20 |
| Fake urgency | 20 |
| Prize or refund bait | 20 |
| Request to pay or send money | 20 |
| Account threat | 15 |
| Shortened link | 15 |
| Pushes you to a private phone number | 10 |
| Unverified link | 5 |

Only the riskiest link on a message adds points.

**Levels:** Low 0 to 29, Medium 30 to 59, High 60 to 100.

**Safe signs lower the score** and are shown on screen: a message that warns "do not share this OTP" (-15), and links that all go to official domains (-10).

**Fairness checks** to avoid false alarms:

- One weak sign on its own stays Low.
- Fewer than three kinds of weak signs stay below High.
- A critical sign (OTP/password request or lookalike link) is never rated Low.

All points, thresholds and the list of official domains can be changed in the **Tune the scoring rules** panel.

## Example results

| Message | Result |
|---|---|
| SBI KYC scam from the problem statement | 100 / 100, High |
| Genuine bank OTP message ("Do not share it with anyone") | 0 / 100, Low |
| College test notice | 0 / 100, Low |
| Empty or very short text | Helpful message, nothing breaks |

The app also understands common Hinglish phrases such as "turant", "block ho jayega" and "OTP batayein".

## Run it

No install and no server. Open `index.html` in any browser. It is a single file of HTML, CSS and JavaScript and works on a phone-sized screen.

## Limits

Scam Spotter gives guidance, not a guarantee. Its rules cover common patterns, so a new kind of scam may not be flagged. If you are unsure, contact the organisation through its official app or website.

## Team

[Add your team name and members here]

## Credits

Built with help from Claude, an AI assistant by Anthropic.
