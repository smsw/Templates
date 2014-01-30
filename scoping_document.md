#Scoping Document for AWebsite.com

Give a brief outline here about the client, project and requirements.

Awebsite.com are a startup with a product called 'Find my fashion'.
It's a website aimed at 16-24 males and females and shows fashion outfits available on high street and they can win the outfit when they've shared it 1000 times.

----

**Min Browser:** IE 10, and the usual

**Framework:** Foundation, Bootstrap

**Platform:** PHP, ExpressionEngine, Statamic

**Third party platform integration:** Facebook, Twitter, YouTube

---

###0. Global

Header and footer appear on all pages unless specified.

- 0.1 Header (header)
  - **0.1.1** Logo (links to home, see 1.)
  - **0.1.2** Links
    - **0.1.2.3** Fashion (/fashion)
    - **0.1.2.4** Win Outfits (/win-outfits)
    - **0.1.2.5** About us (/about)
    - **0.1.2.6** News (/news)
  - **0.1.3a** Login (see 0.a) or Sign Up (see 0.b)
  - **0.1.3b** Logged in (shows welcome, name and avatar), links to account settings
    - **0.1.3b.1** Account settings
    - **0.1.3b.2** Favourite outfits
    - **0.1.3b.3** Logout
  - **0.1.4** Twitter external link (www.twitter.com/Awebsite) 
  - **0.1.5** YouTube external link (www.youtube.com/Awebsite)
  - **0.1.6** Facebook external link (www.facebook.com/Awebsite)

- 0.2. Footer (footer)
  - **0.2.1** Etc

      
###1. Home

*Layout: default*

*Template: home*

*Partials: header, footer, news*

- **1.1** Banner
  - **1.1.1** Show one or more images of the product - will have arrows and bullets to navigate between images.
  - **1.1.2** Show two of the latest news items, including 100x100px image, title, summary and link.
- **1.2** Introduction: Title: An amazing product, Paragraph: Introduction to this amazing product it is wonderful etc...
- **1.3** This weeks winners: three column layout showing 200x200 avatar, name as title and what they won.
- **And so on...**


###2. Fashion

Shows all fashions on page load, if filtering then once submitted goes to results page

*Layout: default*

*Template: fashion*

*Partials: nav, footer, fashion*

- **2.1** Filter Fashion - once submitted goes to /fashion-finder/resutls
  - **2.1.1** Search by colour - dropdown of colours: red, blue, pink, etc)
  - **2.1.2** Search by brand - dropdown of brands: GAP, etc (see brands.doc on server for full list)
  - **2.1.3** Search by price range -£0 - £50, £50 - £100, £100 - £500, £500 - £1000
  - **2.1.4** Search by keyword - input box for keyword entry
  - **2.1.5** Submit button to say 'Find my fashion'
  - **2.1.6** Reset button to say 'Clear filters'

---

*or an alternative version of the same thing*

---

###2. Fashion

Shows all fashions on page load, if filtering then once submitted ajax updates results in same page, When filters are added a box appears saying which filter has been applied - this filter box can be removed by clicking a cross on the filter.

*Layout: default*

*Template: fashion*

*Partials: nav, footer, fashion*

- **2.1** Filter Fashion
  - **2.1.1** Search by colour - dropdown of colours: red, blue, pink, etc)
  - **2.1.2** Search by brand - dropdown of brands: GAP, etc (see brands.doc on server for full list)
  - **2.1.3** Search by price range -£0 - £50, £50 - £100, £100 - £500, £500 - £1000
  - **2.1.4** Search by keyword - input box for keyword entry
  - **2.1.5** Submit button to have magnifying glass icon only and joined to right of keyword box.
- **2.2** Search results - list limit of ten search results
  - **2.2.1** Image, 200x200px
  - **2.2.2** Title
  - **2.2.3** Summary
  - **2.2.4** Link shaped like a boot, saying 'Read on'
- **2.3** Pagination if more than 10 results (see web sheet, pagination design)


