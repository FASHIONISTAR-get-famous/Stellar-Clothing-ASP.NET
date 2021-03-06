# Documentation for Stellar Clothing Website

The project represents an online retailing store for selling clothes. This project doesn't have a real purchasing logic, hence a shopping cart is not entirely implemented. Basically, a user has a variaty of options when surfing through the website. A dropdown menu on the top of the page enables a user to easily navigate through the website. On the first level of the dropdown menu there are categories (e.g MEN,WOMEN). By clicking on an item the dropdown menu shows all submenus which represent subcategories (Accessories, T-Shirts, Skirts...). By clicking on a subitem a user arrives to the page which shows all products that belong to that subcategory. By clicking on a product a user navigates to the page which shows detailed information about the product. On that page a user can rate a product, view product's rates, choose a color or/and a size (if it's available) and an amount and add it to a shopping cart. Finally, when a user decides to buy some products, he proceeds to the shopping cart and finishes shopping.

Front-end technologies used: HTML, CSS, jQuery, JavaScript.

Back-end technologies used: ASP.NET Core, SendGrid API

###### Pages:
1. **Home page** - There's a dynamic slider which consists of images which are fetched from the database. Below slider there are products that have the highest discount. On the bottom of the page (and every other) there is a footer navigation menu which is fetched from the database as well. 

2. **Products page** - A page that contains all products that belong to a previously chosen subcategory from the header menu. On the bottom of the page is a pagination. On the side there is a slider for filtering and a dropdown list for sorting. A user can optionally filter products by moving a slider which represents a price range. There is also a dropdown list which can be used to sort products by a price or a discount.

3. **Single page** - A page which contains all the information about a previously chosen product. A user can rate the product by marking stars. This feature only works for logged users. There is an average rating for a product on the bottom of the page. To add a product to the shopping cart, a user has to choose a quantity before and a color or/and a size (depends on the product). Only logged users can do it.

4. **Checkout page** - A page which contains a list of shopping cart items - products that have been previously added by a user. A user can remove a product from a shopping cart by clicking on a cross on the side or remove all products by clicking on the Delete all button. On the bottom of the page there is a total price. By clicking on the Order button a user finishes his shopping session.

5. **Contact page** - This page represents a place for interacting with the website's administrator. A user (no matter if it's logged in or not) can contact an administrator by filling in the form. Below the form there is an active poll. A user can vote by clicking on one of the options.

6. **Login page** - The place for logging in

7. **Register** - The registration form. After registering, a user must verify his/her email. Sending e-mails with a token for verification purposes is established using SendGrid API.

###### Other pages:
> There are other pages that are auto-generated by model scaffolding. These pages are used for a website administration and aren't entirely completed. Their controllers are stored in AdminPanel folder in Controllers folder.
