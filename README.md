# Take home assignment
  Hello! 👋

  Congratulations on making it to the second round! 
  
## Goal of the task 
  Your goal is to fully test the application using Rspec and Capybara

## Todo list
1) Cover everything with tests where you think is necessary (including model tests, behaviour tests, and etc...)
2) Write tests for "user_order_stats" method in app/models/order.rb

## Set up
```sh
Run bundle exec rake db:seed to populate your database.
```

## How does the application work:

Navigation bar: 
1) “Home link” and “QaTest OneClass link” should direct to the homepage.
2) “Juice” link should direct to /juice URL and show all the juices available in the online store.
3) “Icecream” link should direct to /icecream URL and show all the ice cream available in the online store.
4) “All Categories” link should direct to /all_items.
5) “Login” link should direct to login page.
6) “Signup” link should direct to signup page. 
7) “Logout” link should log out the user and clear his cart. The “Logout” link should only be visible to logged in users.
8) “Cart” link should direct to /my_cart, which is only visible to logged in users AND there is at least one item in the cart. 

Pages:
1) "All Categories" should show all available categories links (/juice and /icecream). 
2) Logout view:
  - Home: should have the text "Login/Signup first"
  - Juice/IceCream: should have list of items with name and image 

3) Logged In view:
  - Home: should have the text: "Navigate to different categories and choose whatever you want" and a list of my successful orders.
  - Juice/IceCream: should show a list of items with name, image and 'Add to Cart' or 'Remove from cart' button.
  - Cart: should be visible to logged in users, and show the following: name, img, 'Remove from Cart' button.

Buttons:  
1) Add to Cart: should add an item to the cart and only visible to logged in users AND this button only appears if the item is not yet added to the cart.
2) Remove from Cart: should remove item from the cart and only visible to logged in users AND this button only appears if item is already in the cart.
3) Order: shows on “my_cart” url only. After user click on it, it should do the following:
  a) Create an order record 
  b) Clean up the user’s cart 
  c) Show success message
  d) Direct to homepage

Items:
1. We should only show the items if the name and image exist. 
2. If there is no name OR the image is broken, this item should be hidden from the list. 


If you're stuck on a bug or something needs clarification you can email [Max](mailto:max@oneclass.com) for help.

Good Luck! 🚀

