# 🛒 E-Commerce Platform

A full-stack e-commerce web application where users can register, log in, browse products, manage their cart, place demo orders, and receive order/shipping updates via email. Admins can manage inventory, update order statuses, and handle product listings.

---

##  Features

###  User Functionality
- User Registration & Login
- Browse all available products
- Search & filter products by category
- Add multiple items to cart
- Increase/decrease item quantity in cart
- Checkout and place orders with demo payment
- View order history with shipping status
- Email notifications for:
  - Successful registration
  - Order confirmation
  - Shipping updates
  - Restock notifications for out-of-stock items

### ️ Admin Functionality
- Admin authentication
- Add, update, and delete products
- Manage product inventory
- View all user orders
- Update order status (Shipped / Delivered)

---

## Tech Stack



**Frontend:**
- HTML, CSS
- JSP (Java Server Pages)

**Backend:**
- Java (Servlets and JSP)
- JDBC (Java Database Connectivity)

**Database:**
- MySQL

**Build & Deployment:**
- Apache Tomcat
- Apache Maven

### ========== GENERATING GMAIL APP PASSWORD [For Mailing Functionalities] ==========
Step 1: Make sure you're logged into your Gmail account and 2-Step Verification is enabled at https://myaccount.google.com/security.

Step 2: Go to https://myaccount.google.com/apppasswords, select "Other (Custom name)", type "Online Electronics", and generate a 16-digit app password — copy and save it for later use.


### ========== Importing and Running The Project Through Eclipse EE ==========

Step 1: Open Eclipse EE.

Step 2: Click On File > Import > Git > Projects From Git > Clone Url > Paste The Repository Url as: ```https://github.com/AlgoSarthak/CS315-Project```> Select master Branch > Next > Next > Finish.

Step 3: Go inside ```Java Resources > src > application.properties```.
- a) Update value for db.username and db.password according to your installed mysql credentials.
- b) Update value for mailer.email and mailer.password, with the same email and app password that you generated earlier in above section 

Step 4: Right Click on Project > Run as > Maven Build > In the goals field enter "clean install" > apply > run

Step 5: Right Click On Project > Build Path > Configure Build Path > Libraries > Remove and Update Any Libraries if Red Mark Exists > Finish.

Step 6: Right Click on Project > maven > update project > select force update > apply > close

Step 7: Tomcat Configurations:
- If Tomcat Server is not configured in Eclipse :
	-  Right Click On Project > Run As > Run On Server > Manually Define a new server > Select server type > select Tomcat v8.0+ > (Select Tomcat V8.0+ Installation Location If Asked) > Next > Add the current project > Finish.

- Else If Tomcat Server is already configured in Eclipse:
	- Right Click On Project > Run As > Run On Server > Select Tomcat Version > Next > Add the project > Finish.
	- You can directly goto server tab, select the tomcat server and use the debug or run button to start the previously ran project

Step 8: Check Running The Site At  [http://localhost:8080/shopping-cart/](http://localhost:8080/shopping-cart/)

Step 9: Default Username And Password For Admin Is "admin@gmail.com" And "admin"

Step 10: The default Username And Password For User Is "guest@gmail.com" And "guest"


