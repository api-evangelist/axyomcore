# AxyomCore

Telecom infrastructure software vendor, styled **Axyom.Core**, supplying cloud-native 4G and 5G
mobile core and RAN network functions (CNFs) that run inside communications service provider
networks. Part of **Lumine Group**, following a carve-out from **Casa Systems**.

- **Website:** https://axyomcore.ai (also holds axyomcore.com, which redirects)
- **Company:** https://axyomcore.ai/about-us
- **News and insights:** https://axyomcore.ai/en/news-insights

## Product lines

| line | page |
|---|---|
| 4G core | https://axyomcore.ai/4g-core |
| Femto core | https://axyomcore.ai/femto-core |
| Security gateway | https://axyomcore.ai/security-gateway |
| RAN | https://axyomcore.ai/ran |
| Full MVNO | https://axyomcore.ai/full-mvnos |

5G core is the headline offering in the site navigation, but no page resolves at `/5g-core`, so it
is not linked here.

Recent public signals: expanded Red Hat OpenShift support, inclusion in Omdia's market landscape
for core networks, and recognition in two Network X award categories.

## No public API surface — and what that does and does not mean

AxyomCore publishes **no developer portal, no API documentation, and no machine-readable
contract**. Verified 2026-08-17:

- the advertised `https://axyomcore.ai/apis.json` returns **404**
- `developer.axyomcore.ai`, `docs.axyomcore.ai` and `api.axyomcore.ai` do **not resolve**
- `llms.txt` returns **404**
- the word "api" appears **zero times** on the homepage
- the site is HubSpot-built, and the primary call to action is **Submit RFP**

**This is the absence of a PUBLIC interface, not the absence of APIs.** A 4G/5G mobile core is
API-driven by construction — 3GPP service-based architecture is defined in terms of HTTP/2 and
JSON service interfaces, and any CNF deployed on Kubernetes exposes management and orchestration
interfaces to the operator running it. Those interfaces reach customers under operator contracts
and RFP engagements rather than through a public developer program, so a public catalog cannot
index them.

The Kin Score reflects what is publicly discoverable. For a vendor selling into carrier networks
that number will be low, and it should be read as a measure of public developer surface rather
than of engineering quality.

## Why this is listed

The intake gate parked this submission as `no_consumable_surface`. It is listed anyway, on the
standing rule that **a valid company on a domain it owns gets a listing and a low score** — the
score is what gives a vendor something to improve against. Roughly half of the providers in this
catalog carry no `apis[]` entry.

No contract, endpoint, or specification was invented to fill the gap. `apis[]` is empty because
there is nothing public to put in it.

---

*Profiled by [API Evangelist](https://apievangelist.com) · listed on [APIs.io](https://apis.io) ·
reviewed 2026-08-17*
