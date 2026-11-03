# Tessera Linux launch checklist

## Immediate Early Access beta

- [x] Cross-platform pure-Kotlin game engine carried into desktop build
- [x] Mouse input, last-piece/refill and line-clear animation regression suite
- [x] Isolated production CSC house-ad catalog deployed separately from Stripe
- [x] Early Access build configuration: no test billing or test multiplayer buttons
- [x] Separate early-access local-save directory
- [x] Installable binary, checksum and portable archive built and verified
- [x] UI/advertisement QA in isolated user profile
- [x] Owner approved publication of v0.6.0-beta1 on 2026-11-02
- [x] Public v0.6.0, v0.6.1 and v0.6.2-beta1 GitHub releases published; v0.6.2 checksum independently downloaded and matched
- [x] Publish Early Access privacy notice on CSC site; online version updated for GitHub release checks
- [ ] Owner/legal review of published privacy notice before paid public launch

## Full paid/cross-platform production version

- [x] Provision separate production D1 and Commerce Worker; deployed fail-closed and awaiting live secrets
- [x] Deploy dedicated production Live Duel Worker, Durable Object namespace and rate limiter, **PUBLIC_MATCHES_ENABLED=false**; entitlement acceptance tests pending
- [ ] Obtain **restricted Stripe live key** and **signed live webhook secret** through secure installation, never chat
- [x] Draft live Stripe $0.99 and $2.99 one-time products, held inactive until rollout
- [ ] Enable products and signed webhooks *after* server-side live verification
- [x] Implement one-time code recovery backend, password resets and prior-session invalidation; local tests pass
- [ ] Add production account recovery UI and finalize buyer/support/privacy terms
- [x] Test signed webhook replays, refunds/disputes and account-bound restore with mocked Stripe API in offline production-unit tests
- [ ] Run actual signed Stripe live-mode webhook, refunds/disputes and game-level purchase tests against production
- [x] Implement official-release check UI and repeatable, fail-closed release build script; publish v0.6.2-beta1
- [x] Validate package installation and headless launch on clean Ubuntu 24.04/Debian 13 containers (GPU driver-dependent real GUI QA pending)
- [ ] Test Android production app versus desktop production (no staging URLs)
- [ ] Owner reviews legal/privacy policy and approves live payment activation

## Distribution follow-up (November 3, 2026)

The versioned CSC landing page at https://www.casesensitivecomputers.com/tessera/ serves v0.6.2-beta1. The apex address https://casesensitivecomputers.com/tessera/ still serves older cached HTML without a cache-busting query, while an apex query parameter returns the new Worker; an upstream cache/route conflict remains to be resolved without disrupting the separate production CSC website. Keep official user-facing links on `www` until fixed.

The free beta is **not** the paid/production desktop channel. Do not activate live checkout or Live Duel until the remaining production security gates are verified.
