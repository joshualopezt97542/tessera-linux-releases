# Tessera Linux launch checklist

## Immediate Early Access beta

- [x] Cross-platform pure-Kotlin game engine carried into desktop build
- [x] Mouse input, last-piece/refill and line-clear animation regression suite
- [x] Isolated production CSC house-ad catalog deployed separately from Stripe
- [x] Early Access build configuration: no test billing or test multiplayer buttons
- [x] Separate early-access local-save directory
- [ ] Installable binary, checksum and portable archive built and verified
- [ ] UI/advertisement QA in isolated user profile
- [ ] Owner approves Early Access scope and public privacy language
- [ ] Publish on an official, owner-controlled download page or GitHub Releases

## Full paid/cross-platform production version

- [ ] Provision production D1 and separate Commerce Worker (never point users at staging)
- [ ] Provision dedicated production Live Duel Worker with Android Google Play and desktop Stripe host entitlements
- [ ] Obtain **restricted Stripe live key** and **signed live webhook secret** through secure installation, never chat
- [x] Draft live Stripe $0.99 and $2.99 one-time products, held inactive until rollout
- [ ] Enable products and signed webhooks *after* server-side live verification
- [ ] Implement account recovery, security controls and support/transaction policy
- [ ] Test refund/dispute revocation, duplicate webhooks, entitlement restore and game-level purchase behavior
- [ ] Configure automated update/distribution and validate on clean Ubuntu/Debian machines
- [ ] Test Android production app versus desktop production (no staging URLs)
- [ ] Owner reviews legal/privacy policy and approves live payment activation
