# OverRich – Smart Streetwear Fashion Website

Frontend for **OverRich**, a streetwear brand selling premium oversized T-shirts. Built as a single, dependency-light page (HTML, CSS and vanilla JavaScript) with AOS scroll animations.

## Features
- Home page with hero carousel, sale banner with countdown, collections, categories, trending and new-arrival sliders, smart size finder, limited-edition drop, lookbook, reviews and newsletter
- Dedicated pages: Shop (filters by collection, colour, size, fit, sleeve, design, finish, price), New arrivals, Trending, Limited edition, Collections, Lookbook, Custom design, Wishlist, Bag, My orders, Track order, My account, Store admin
- 34 styles in 15 colours across 7 collections, with photo-style product renders (flat lay, back, hanger, folded, close-up)
- Light and dark themes, fully responsive down to phone width

### Stage 2: e-commerce features
- **Accounts:** sign up and log in with email and password. Passwords are stored as salted PBKDF2-SHA256 hashes, sessions last 7 days, and 5 wrong attempts lock the email for a minute
- **Profile:** edit name and mobile, address book (add, edit, delete, set default), change password, fit profile and email preferences
- **Cart:** saved per account; choose size, colour and quantity; edit or remove items; subtotal and estimated order amount; quantities limited by stock
- **Checkout:** delivery details → order summary review → confirm. Cash on delivery only (no payment gateway in this stage)
- **Order status:** unique order IDs; Pending → Confirmed → Processing → Shipped → Delivered (or Cancelled) with a dated history. Customers can cancel while Pending or Confirmed; guests can track with order ID and mobile number
- **Admin panel** (`#admin`): update order status manually, and manage stock per product and size
- **Wishlist:** save favourites and move them to the bag
- **Size recommendation:** from height and weight, shown on products, quick add, bag and the checkout review
- **Reviews and ratings:** only for products in a delivered order; edit or delete your own review

## Admin login
- Email: `admin@overrich.in`
- Password: `Admin@2026` (change it from My account → Password)

## Run locally
Open `index.html` in a browser. No build step.

> Demo only: there is no server yet. Accounts, orders, stock and reviews are stored in the visitor's browser (localStorage), so an admin on another device won't see a customer's orders.
