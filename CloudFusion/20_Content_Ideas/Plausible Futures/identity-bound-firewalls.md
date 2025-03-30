Title: What If Your Firewall Knew Who You Were?

Concept:
Can we push identity information (Entra user/device) down to the firewall layer?

Instead of IP → IP rules, we define rules like:
ALLOW: `HR Group` to access `Payroll App`
BLOCK: `Contractor Devices` from `Internal Fileshare`

This would effectively blend cloud IDP + LAN segmentation.

Tech blockers:
- Can identity tokens be passed to OPNsense?
- Requires custom Radius/LDAP/OpenID link?

Totally wild. But maybe not.
