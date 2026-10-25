# Example walkthrough: a web login flow

**System:** a standard login flow for a web app.
**Closed World:** existing components of the flow plus the user's existing device and email. No new hardware, no new third-party service.

## Inventory
Components: username field, password field, MFA code step, "forgot password" link, session cookie, login page, error message.
Attributes: strictness of checks, timing of authentication, number of steps, where the user is, which device is used.

## Variants

| # | Component | Tool | New configuration | Beneficiary & function | Feasibility | Main risk |
|---|---|---|---|---|---|---|
| 1 | Password field | Subtraction | Remove the password field; sign-in is a one-time link to the user's existing email | Users who forget passwords; fewer reset requests | High | Email account becomes a single point of failure |
| 2 | Session cookie | Task Unification | The cookie also carries a rolling trust signal that is re-checked during the session | Security teams; catches hijacked sessions | Medium | Complexity, false positives |
| 3 | Password field | Multiplication | A second, different password that opens a limited "duress" view | Users under coercion | Medium | Needs careful design to avoid misuse |
| 4 | Login step | Division | Split login in time: browse anonymously, authenticate only on sensitive actions | Users who just want to look around | High | Inconsistent experience if poorly signposted |
| 5 | MFA step | Attribute Dependency | MFA strictness depends on device and location | Frequent users on trusted devices | High | Attackers may imitate "trusted" context |

## Notes
Several of these ideas already exist in some form in the market (passwordless links, step-up authentication, risk-based MFA). That is expected: SIT patterns describe how many past inventions were built, so rediscovering them is a sign the method is working. The most interesting rows to explore further are usually the ones that feel slightly odd, such as #3.

Feasibility ratings are rough judgments, not validated figures.
