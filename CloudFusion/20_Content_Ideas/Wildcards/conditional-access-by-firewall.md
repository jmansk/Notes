## Conditional Access from the Firewall Side

Can we flip the model?

- Instead of Entra ID doing CA based on location…
- What if Shield enforced firewall access **based on Entra identity group membership**?

Wild but worth thinking about. Might require:
- LDAP sync with Azure
- OPNsense plugin or API integration
- External RADIUS server bound to Entra

Why it matters:
- Merges cloud trust + LAN segmentation
- Allows dynamic firewall rules per user group
