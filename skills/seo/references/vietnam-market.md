# Vietnam Market Profile (Bống Media configuration)

Load this file for every command when the site is Vietnamese (`.vn` domain,
`lang="vi"`, Vietnamese body text, `+84` phone numbers or a Vietnamese
address), or when the user writes in Vietnamese.

## Output language

- Write every report, action plan, brief and chat summary in **Vietnamese**,
  with full diacritics, unless the user asks for another language.
- Keep standard SEO terms in English where Vietnamese marketers use them
  (SEO, SERP, schema, canonical, Core Web Vitals, E-E-A-T, backlink,
  anchor text), and explain each the first time it appears in a report.
- Severity labels: Nghiêm trọng (Critical), Cao (High), Trung bình (Medium),
  Thấp (Low). Keep the scoring method unchanged.
- Code, JSON-LD, file names and commands stay in English.

## Search landscape

- Google is the dominant search engine in Vietnam; treat it as the primary
  target. Mention Cốc Cốc (browser and search) only as a secondary check.
- Searchers type both with and without diacritics ("dịch vụ seo" and
  "dich vu seo"). Keyword research and clustering must group both forms as
  one intent, and titles/headings should carry the accented form.
- Mobile traffic dominates: weight mobile rendering, tap targets and INP
  above desktop findings.
- Zalo and Facebook are the main contact and trust channels. Check that the
  site links a Zalo contact or Zalo OA and the Facebook fanpage, and that
  click-to-call works on mobile.

## On-page conventions

- URL slugs: lowercase, no diacritics, hyphen separated
  (`/dich-vu-quang-cao-facebook`, not `/dịch-vụ-...` or `%E1%BB%8B`).
  Flag percent-encoded Vietnamese slugs as a Medium issue.
- `<html lang="vi">`; for multi-language sites use hreflang `vi` or `vi-VN`
  plus `x-default`.
- Title tags: Vietnamese is longer per keyword; judge truncation by pixel
  width, not character count, and put the main keyword first.
- Check that fonts render Vietnamese diacritics correctly (no fallback
  glyphs for ầ, ặ, ữ, ợ) in screenshots.

## Local SEO in Vietnam

- Administrative reform effective 1 July 2025: provinces were merged
  (63 → 34 provincial units) and the district level (quận/huyện) was
  removed, so many addresses changed. Example: Hải Dương province merged
  into Hải Phòng city. Flag any NAP (name, address, phone) still using the
  old province or district on the site, Google Business Profile, schema
  and directories, and recommend one consistent new-format address.
- Phone numbers: show local format (0968 xxx xxx) on the page, use
  `+84` international format in schema `telephone`.
- Schema: `addressCountry: "VN"`, `priceCurrency: "VND"`,
  `inLanguage: "vi"`.
- Citation sources worth checking: Google Business Profile, Facebook page,
  Zalo OA, trangvangvietnam.com, industry directories, and Foody for
  food and drink businesses.

## Trust signals (E-E-A-T)

- Company legal name (Công ty TNHH / Cổ phần ...), tax code (mã số thuế),
  registered address and hotline in the footer or About page.
- Websites that sell online or take orders should show the Ministry of
  Industry and Trade registration badge (online.gov.vn); flag it as missing
  on e-commerce sites and treat it as a trust gap, not a ranking factor.
- Real photos of team, office, projects and customers outweigh stock images.

## E-commerce

- Main marketplaces: Shopee, Lazada, TikTok Shop, Tiki. When a brand also
  sells there, check that product names and prices stay consistent with the
  website and that the website has richer product content.

## Site profiles

Bống Media's own sites: see `bongmedia-sites.md`.
