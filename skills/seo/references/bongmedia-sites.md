# Bống Media Site Profiles

Known sites for this installation. When the user names a site by brand
("audit Bống Media", "kiểm tra XSHD") use the matching URL without asking.
Apply `vietnam-market.md` to all of them.

| Brand | URL | Notes |
|-------|-----|-------|
| Bống Media (Công ty TNHH Bống Media) | https://bongmedia.vn | Company site. Detect business type from the homepage. |
| XSHD - Xuân Sơn Hải Dương | https://xshdsolar.vn | Solar power (điện mặt trời) information site. WordPress, Elementor-based theme, Vietnamese only, no shopping cart. Hotline 0968 885 558. |

## Per-site checks

**bongmedia.vn**
- Check that the Facebook fanpage and the site link to each other.

**xshdsolar.vn**
- Treat as a local service business: run local SEO checks and suggest
  `/seo local` after a full audit.
- Address uses the Hải Dương name: verify it follows the post-July-2025
  administrative format (now part of Hải Phòng city) everywhere (site,
  Google Business Profile, schema, directories).
- WordPress: check that the SEO plugin (Rank Math or Yoast) outputs a
  single canonical, a valid XML sitemap, and no duplicate JSON-LD.
- Since there is no cart, do not recommend Product or Offer schema;
  prefer `LocalBusiness` (or a subtype) and `Service`.

To add a site, append a row to the table above and push to the fork.
