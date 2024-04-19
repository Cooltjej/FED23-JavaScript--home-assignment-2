### A simple webshop using javascript  

You are to collaborate in groups of 3 to create a simple webshop where users can add products to a shopping cart and then proceed to "checkout" and place an order.  

-------------------------------------------------------------------  

### Requirements Specification  

As mentioned, you are to create a simple webshop that interacts with an API I have set up, where users can retrieve products to add to a shopping cart and then place an order (via a POST request to an API endpoint I have also set up).
  
Upon visiting the page, all products should be displayed with a thumbnail image, name, price, and an "Add to Cart" button.
  
The shopping cart should be displayed with a collapsible summary on the page, showing all products (and quantities of each product) that have been added to the cart.
  
If a user clicks "Add to Cart" on a product that is already in the cart, the quantity of the product should increase, but only 1 should be displayed in the cart alongside the quantity. It should also be possible to remove a product from the cart.
  
Users should also be able to click on a product (preferably through a "Read more" link) and view more information about the product (large image, name, price, description), without losing the shopping cart.  
  
The shopping cart should be saved in Local Storage so that it persists even after page reloads.
  
In the shopping cart, there should be a "Proceed to Checkout" button that leads to a new view where users can fill in the following details (the underlined ones should be required):  

Name  

Address  

Postal code (max 6 characters)  

City  

Phone number  

Email  

When placing the order, any errors should be displayed, and if the order is successful, the order number should be displayed along with a thank-you message.  

-------------------------------------------------------------------  

### Hygiene Requirements  

The following hygiene requirements must be met regardless of the grade level.  

Be responsive (mobile-first, with at least 3 different layouts).  

Semantically correct HTML.  

Use flexbox or CSS grid (using Bootstrap/Tailwind etc. is also acceptable).  

Styled adequately (i.e., look decent without spending too much time on it).  

All data and status should be managed in JavaScript, i.e., do not use the DOM as the single point of truth.  

Written in TypeScript and using Vite.  

Communication with the API should occur in a separate module.  

Data types should be defined for the API (both for the response you receive and the data you send).  

Published via Netlify/GitHub Pages/Vercel.  

-------------------------------------------------------------------  

### Update 2023-12-22  

The client has reached out (typical clients to do so on a Friday afternoon 🙄) and wants the following additions:  

The number of products should be displayed in the product overview, e.g., "Showing 137 products" (should be dynamically updated, i.e., not hardcoded).  

The shopping cart should display the total for each product (quantity * unit price) as well as the order total both in the shopping cart and at checkout.  

###  Update 2023-12-28  

New week, new requirements 😁  

The client is thrilled with the previous changes but has realized after the Christmas sales (typical clients! 😅) that candy can run out 😱!    
  
Therefore, they (me 😝) want you to implement support for:  

Sorting products by product name.  

Products that are out of stock (stock_status: "outofstock") should be displayed but not be able to be added to the shopping cart (e.g., the "Add to Cart" button should be disabled).  

The number of products in stock should be displayed (e.g., "Showing 137 products, of which 42 are in stock") along with the total number of products in the overview of all products.  

Display the stock quantity (stock_quantity) of each product (when the visitor views the product details).
