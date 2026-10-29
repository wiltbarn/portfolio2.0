vanessabarron.fyi — site files
==============================

WHAT'S HERE
  index.html                  Home page (hero, work cards, resume, contact)
  email-sms-campaigns.html    Email & SMS campaigns page (3 campaigns, finished)
  automation-bot.html         COB / Automation bot page (finished, linked from the card)
  tasting-table.html          Writing page with filler text (not linked yet)
  pan-m-360.html              Writing page with filler text (not linked yet)
  secret-media.html           Writing page (formerly Secret Media)
  css/styles.css              All styling for every page (colors are at the top)
  images/                     Photos, screenshots, logo, and icons
  files/                      Resume PDF (resume.pdf)
  favicon.ico, robots.txt, sitemap.xml

HOW TO PUBLISH
  Upload everything, keeping the folder structure: the css/ and images/ folders
  must sit next to index.html. If pictures are missing on the live site, check
  that www.vanessabarron.fyi/images/hero.jpg opens. index.html must sit at the
  top level so the home page opens at the address.

PAGE LINKS
  Pages are linked with their .html name (for example
  /email-sms-campaigns.html), which works on any host. The site address used in
  canonical tags, sharing tags, sitemap.xml and robots.txt is
  https://www.vanessabarron.fyi. If you move to a different address, search the
  files for it and update.

BEFORE YOU GO LIVE (search the files for "TODO" and for "[")
  1. Resume PDF: done (files/resume.pdf). To update it, replace that file and keep the name.
  2. About page: once about.html exists, add the "Learn more about me →" link to the intro (see the TODO in index.html). The radio show link will live there.
  3. Cards for Automation bot, Blog design & content, Tasting Table, PAN M 360 and
     Secret Media say "Coming soon" because those pages don't exist yet.
     Two cards still have [bracketed] placeholder captions (
     Tasting Table).

ADDING A PROJECT PAGE (or linking one of the filler pages above)
  Copy email-sms-campaigns.html, rename it (e.g. automation-bot.html), edit the
  text, then in index.html replace the card's "Coming soon" span with:
    <a class="more" href="/automation-bot.html" aria-label="Learn more about Automation bot">Learn more →</a>
  and add the page to sitemap.xml. The four filler pages are not in sitemap.xml
  and their cards still say "Coming soon" so the filler text stays out of sight
  until you have filled them in. Dashed boxes marked [Picture] stand in for
  images: replace the whole <div class="placeholder"> with an <img> tag.

TESTING ON YOUR COMPUTER
  Opening the files by double-click won't show the logo (browsers block it for
  local files) or follow the page links. Instead, open a
  terminal in this folder, run:  python3 -m http.server
  and visit http://localhost:8000

ARTICLE PAGE FORMAT: every project/article page has title, hero drawing, intro (lede), then the
facts card (Role, Company, Timeline, Tools) before the sections. Copy the <dl class="facts"> block.

OPEN ITEM: secret-media.html -- add Google Analytics performance numbers if you find them (search for TODO). Also fill in Role and Timeline there.

OPEN ITEM: card captions on index.html contain ## placeholders (Automation bot influencer count; Product & ad copy customers and ROAS). Search for "##".

product-ad-copy.html is live (linked from the card, in the sitemap). Open items: add February BeatBuddy 2 and June Aeros ROAS if you find them.

social-media.html is live (linked from the card, in the sitemap). Open items: add scheduling/design tools to the facts box (search for TODO); optionally draw a bigger header image (images/header-social-media.png is the card art reused).

about.html is live (noindex removed, in sitemap, linked from the home page). Open items: radio show details and link (search for TODO), and rewrite the text in your own voice.
