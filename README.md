SOLANA TEC GRAND OPENING — MOBILE EVENT GUIDE
==============================================

A mobile-first bilingual landing page created for the Solana Tec Grand Opening on 21 November 2026.

Visitors can access the event guide by scanning a QR code. The website provides the event programme, an interactive floor plan, station locations and partner logos.

FEATURES
--------

- Mobile-first responsive design
- English and Mandarin language options
- Interactive event floor plan
- Ten clickable event booths
- Event programme and station pause times
- Automatic event countdown/status
- Light and dark mode support
- Reduced-motion accessibility support
- Solana Tec mascot animations
- Partner and sponsor logos
- Optimized image assets
- Cloudflare Pages compatible
- No frameworks or build process required

EVENT STATUS
------------

The event status changes automatically using Malaysia time:

Before 21 November 2026:
“3 days to go”, “2 days to go”, etc.

21 November 2026, before 10:00 AM:
“Happening today”

21 November 2026, 10:00 AM–2:30 PM:
“Happening now”

After 2:30 PM:
“Thank you for joining us”

Mandarin translations are displayed when the user selects 中文.

PROJECT STRUCTURE
-----------------

index.html
    Main website containing the layout, styling, translations and interactions.

assets/
    site/
        solana-tec-logo.png
        floor-plan.webp

        mascots/
            mascot-megaphone.webp
            mascot-thumbs-up.webp

        partners/
            pylontech.png
            helukabel.png
            ja-solar.png
            power-stone.png
            re-energy.png

cloudflare-deploy/
    Deployment-ready version of the website.

solanatec-grand-opening-cloudflare.zip
    ZIP package ready for Cloudflare Pages Direct Upload.

LOCAL TESTING
-------------

The page can be opened directly using index.html.

For more accurate testing, run a local web server from the project directory.

Example using Node.js:

npx serve .

Then open the local URL shown in the terminal.

Recommended mobile test viewport:

Width: 440px
Height: 956px
Device reference: iPhone 16 Pro Max

CLOUDFLARE DEPLOYMENT
---------------------

1. Sign in to Cloudflare.
2. Open Workers & Pages.
3. Create a new Pages project.
4. Select Direct Upload.
5. Upload either:

   - The cloudflare-deploy folder, or
   - solanatec-grand-opening-cloudflare.zip

6. Deploy the project.

No build command, framework preset or environment variables are required.

UPDATING THE WEBSITE
--------------------

Make changes to the main index.html and assets/site directory first.

Before deployment:

1. Copy the updated index.html into cloudflare-deploy.
2. Change asset paths from:

   assets/site/

   to:

   assets/

3. Copy any new assets into cloudflare-deploy/assets.
4. Rebuild the Cloudflare ZIP.
5. Confirm that all images and interactive elements work before uploading.

LANGUAGE SUPPORT
----------------

The language selector is located in the website header:

EN / 中文

The selected language is saved in the visitor’s browser and remains selected when the page is reopened.

INTERACTIVE MAP
---------------

The floor plan uses the official Marketing map at its original proportions.

Transparent interactive hotspots are positioned over Stations 1–10. Selecting a booth highlights its location and displays the station name and location information below the map.

PARTNERS
--------

- Pylontech
- HELUKABEL
- JA Solar
- Power Stone
- RE Energy

Pylontech is displayed as the featured partner at the top of the partner section on mobile devices.

TECHNOLOGY
----------

- HTML5
- CSS3
- Vanilla JavaScript
- Responsive CSS media queries
- LocalStorage for language preference
- WebP and PNG image assets
- Cloudflare Pages static hosting

No external JavaScript libraries or frameworks are required.

BROWSER SUPPORT
---------------

The website is designed for current versions of:

- Google Chrome
- Safari
- Microsoft Edge
- Firefox
- Android browsers
- iOS Safari

CREDITS
-------

Website: Solana Tec Grand Opening Event Guide
Event date: 21 November 2026
Location: Impian Emas, Johor Bahru
Organization: Solana Tec
