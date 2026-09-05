<!-- Replace ORG_NAME below with your GitHub organization handle (one occurrence). -->

<div align="center">

<a href="https://www.mecverse.com/">
  <img src="https://images.weserv.nl/?url=www.mecverse.com/mecversewhitenew.png&w=680&h=180&fit=contain&cbg=ffffff&bg=ffffff&output=png" alt="Mecverse" width="300">
</a>

<br><br>

<img src="https://raw.githubusercontent.com/ORG_NAME/.github/main/profile/assets/Signal.svg" alt="FlowTux · WorkClave · HZRelay" width="100%">

<br>

[![Website](https://img.shields.io/badge/mecverse.com-09090B?style=for-the-badge&labelColor=09090B)](https://www.mecverse.com/)
[![Products](https://img.shields.io/badge/Products-09090B?style=for-the-badge&labelColor=09090B)](https://www.mecverse.com/products)
[![Docs](https://img.shields.io/badge/Docs-09090B?style=for-the-badge&labelColor=09090B)](https://www.mecverse.com/documentation)
[![Demo](https://img.shields.io/badge/Request_Demo-FFFFFF?style=for-the-badge&labelColor=FFFFFF&color=FFFFFF)](https://www.mecverse.com/contact#schedule)

</div>

<br>

<h2>
<img src="https://www.mecverse.com/flowtux_favicon.svg" width="22" align="top">&nbsp;
<a href="https://www.mecverse.com/products/flowtux">FlowTux</a>
</h2>

**AI internal support for every team.**

Slack DMs, Sentry errors, GitHub issues, and email land in one tracked queue. Tux AI
auto-resolves **73%** of tickets and routes the rest in **23ms** by content and business impact.

```
Raise ──▶ Triage ──▶ Dedup ──▶ Route ──▶ Resolve ──▶ Track
```

- **Slack intake** — messages become structured tickets without leaving the channel
- **Sentry triage** — duplicates collapse semantically so real signal isn't buried
- **GitHub sync** — bidirectional, so tickets and code stay in lockstep
- **Smart routing** — auto-assigned to on-call, priority set by business impact

Flat **$99/month**, unlimited members, no per-agent seat tax.

[Product](https://www.mecverse.com/products/flowtux) · [Docs](https://www.mecverse.com/documentation/flowtux) · [flowtux.com](https://www.flowtux.com/)

<br>

<h2>
<img src="https://www.mecverse.com/workclave-logo.svg" width="22" align="top">&nbsp;
<a href="https://www.mecverse.com/products/workclave">WorkClave</a>
</h2>

**Attendance verification and session analytics for teams that need reliable records.**

Captures attendance and engagement from remote sessions, then turns them into reports
teams can review for payroll and compliance.

- **Attendance verification** — reviewable session-presence records
- **Engagement records** — participation trends, session by session
- **Payroll-ready reporting** — exports for reconciliation
- **Audit trails** — traceable records for compliance review

Built for education teams, distributed operations, and compliance workflows.

[Product](https://www.mecverse.com/products/workclave) · [Docs](https://www.mecverse.com/documentation/workclave)

<br>

<h2>
<img src="https://www.mecverse.com/hzrelay-logo.svg" width="22" align="top">&nbsp;
<a href="https://hzrelay.mecverse.com">HZRelay</a>
</h2>

**The routing layer between your app and every real-time provider.**

Voice, tokens, and webhooks normalized to one session model, one SDK. We own codecs,
reconnects, and routing — you own what you're actually building.

```
[ SOURCES ]             [ ROUTER ]                  [ SINKS ]

Twilio · Plivo         codec · reconnect       Deepgram · ElevenLabs
WebRTC · WebSocket ──▶  route · VAD · trace ──▶  OpenAI · Cartesia
Stripe · GitHub                                Anthropic · Your app
```

```ts
import { createSession } from '@hzrelay/sdk'

const session = await createSession({
  inbound: { type: 'twilio' },                 // or 'plivo' | 'webrtc'
  stt: { provider: 'deepgram',   apiKey: env.DG },
  tts: { provider: 'elevenlabs', apiKey: env.EL },
})

// codecs, reconnects, VAD — handled. bring your own agent loop:
session.on('transcript', ({ text, isFinal }) => {
  if (isFinal) session.speak(myLLM(text))
})
```

Per-session latency traces across every hop, provider comparison data, and auto-failover
on SLA breach. Swap providers in config, not in code.

[Site](https://hzrelay.mecverse.com) · [Docs](https://hzrelay.mecverse.com/docs) · [Pricing](https://hzrelay.mecverse.com/pricing)

<br>

## On this GitHub

The public surface of the portfolio — the parts teams integrate against. Product cores stay internal.

| Repository | Purpose |
| :--- | :--- |
| `hzrelay-sdk` | TypeScript SDK for voice, token, and webhook routing |
| `flowtux-agent` | Device agent for telemetry and safe, allow-listed fixes |
| `mecverse-docs` | Source for the public documentation site |
| `examples` | Reference integrations across the portfolio |

Security issues go to [contact](https://www.mecverse.com/contact), not a public issue.

<br>

---

<div align="center">

<sub>NVIDIA Inception Program · Microsoft for Startups</sub>

<sub>

[Company](https://www.mecverse.com/company) · [Careers](https://www.mecverse.com/company/careers) · [Contact](https://www.mecverse.com/contact) · [LinkedIn](https://www.linkedin.com/company/mecverse-tech-solutions)

</sub>

<sub>© 2026 Mecverse Tech Solutions LLP</sub>

</div>
