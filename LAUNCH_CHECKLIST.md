# Launch checklist

## Preview gate

- [ ] Desktop visual QA
- [ ] Mobile visual QA
- [ ] All external links verified
- [ ] Booking email confirmed
- [ ] Release and venue credits approved
- [ ] GitHub Pages preview approved by Juan

## Domain cutover

The current apex domain still points to Cargo. Only change DNS after preview approval.

1. Configure `lagunamusic.co` as the custom domain in GitHub Pages.
2. Add `CNAME` to this repository.
3. Replace the current apex DNS records with GitHub Pages A records.
4. Point `www` to `juanclopez95.github.io` using CNAME.
5. Verify both apex and `www` resolve correctly.
6. Enable HTTPS enforcement after the certificate is issued.
7. Preserve the Cargo configuration until the new site is verified.

## Rollback

Restore the previous Cargo DNS records:

- `3.234.189.133`
- `3.215.100.79`

