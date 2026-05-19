# Launch Setup Notes

## Domain

- Domain: `blossomland.com.au`
- Registrar: GoDaddy
- DNS and email host: Bluehost
- Preferred canonical domain: `https://blossomland.com.au`

## Requested mailboxes

- `hello@blossomland.com.au`
- `sisly@blossomland.com.au`
- `jenks@blossomland.com.au`

## GitHub Pages DNS records

If Bluehost is authoritative for DNS, point the apex domain to GitHub Pages with these records:

- `A 185.199.108.153`
- `A 185.199.109.153`
- `A 185.199.110.153`
- `A 185.199.111.153`
- `CNAME www -> jenksyguo.github.io`

## Email hosting

Create the three mailboxes in Bluehost Email or cPanel Email Accounts.
Preserve Bluehost-provided MX, SPF, and DKIM records for the domain after the nameserver switch.

## Verification checklist

- GitHub Pages custom domain set to `blossomland.com.au`
- DNS resolves to GitHub Pages IPs
- `www` redirects or aliases to the apex domain
- Email accounts exist and can log in
- MX, SPF, and DKIM validate after DNS propagation
