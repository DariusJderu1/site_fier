# Remat - Scrap Metal Collection Website

A responsive, static presentation website built for a local scrap metal collection and recycling business. It provides potential clients with information about services, accepted materials, pricing, and includes an interactive payout calculator.

## Live Demo
[View the live website here](https://dariusjderu1.github.io/site_fier/)

## Key Features & Technical Details

* **Local SEO Ready:** Includes embedded Structured Data (`application/ld+json` / `RecyclingCenter` schema) to help search engines like Google better understand the business location, working hours, and contact details.
* **Interactive Calculator:** A custom Vanilla JavaScript calculator that dynamically computes the estimated payout in real-time based on user input (material type and weight). 
* **Responsive Design:** Built on top of the Bootstrap 5.3.8 grid system, navigation components, and a custom overlay slider (Carousel).
* **Custom Media Queries:** Supplements Bootstrap's default grid with custom CSS `@media` queries to fine-tune typography scaling, padding adjustments, and layout behavior specifically for mobile and tablet viewports.
* **Modern CSS:** Utilizes native CSS features like `clamp()` for fluid typography and flexible element sizing across different screen resolutions.

## Tech Stack

* **HTML5:** Semantic markup and meta tags for basic SEO.
* **CSS3:** Custom styles layered over Bootstrap.
* **JavaScript (ES6+):** Vanilla JS for the calculator logic and DOM manipulation (handling the mobile navbar on outside clicks).
* **Frameworks/Libraries:** Bootstrap 5.3.8

## Project Structure

* `index.html` - The main landing page (Hero, About Us, Pricing, Contact).
* `calculator.html` - Dedicated page for the interactive price calculator.
* `/css` - Contains the custom stylesheets (`acasa.css`, `calculator.css`).
* `/js` - Contains the logic for the navbar (`acasa.js`) and the price calculator (`calculator.js`).
* `/images` - Local image assets used across the site.

## Note on Development
This is a static front-end project. The material prices in the calculator are currently hardcoded in a configuration object within `calculator.js` (`const PRICES = {...}`). For a production environment with frequently changing prices, this logic would ideally be decoupled and fetched dynamically via an API.
