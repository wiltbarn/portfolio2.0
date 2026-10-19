vanessabarron.fyi — site files
==============================

WHAT'S HERE
  index.html                  Home page (hero, work cards, resume, contact)
  email-sms-campaigns.html    Email & SMS campaigns page (3 campaigns)
  css/styles.css              All styling for every page (colors are at the top)
  images/                     Photos, screenshots, logo, and icons
  files/                      Put your resume PDFs here (see below)
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
  1. Resume PDFs: save them in files/ as marketing-resume.pdf,
     writing-resume.pdf and complete-cv.pdf (or edit the links in index.html).
  2. The "internet radio show" link in the intro currently points to #.
  3. Cards for Automation bot, Gear Tribune Blog, Tasting Table, PAN M 360 and
     Boston Uncovered say "Coming soon" because those pages don't exist yet.
     Two cards still have [bracketed] placeholder captions (Gear Tribune Blog,
     Tasting Table).

ADDING A PROJECT PAGE
  Copy email-sms-campaigns.html, rename it (e.g. automation-bot.html), edit the
  text, then in index.html replace the card's "Coming soon" span with:
    <a class="more" href="/automation-bot.html" aria-label="Learn more about Automation bot">Learn more →</a>
  and add the page to sitemap.xml.

TESTING ON YOUR COMPUTER
  Opening the files by double-click won't show the logo (browsers block it for
  local files) or follow the page links. Instead, open a
  terminal in this folder, run:  python3 -m http.server
  and visit http://localhost:8000
