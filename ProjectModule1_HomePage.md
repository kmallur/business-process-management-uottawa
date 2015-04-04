# Home Page in Library Management Process #

![http://i.imgur.com/hJ0c01v.jpg](http://i.imgur.com/hJ0c01v.jpg)

This page is like a 'Welcome Page' to the user.

This page offers the user to perform two major activities:

(i) To borrow item(s)(books/DVDs)
(ii) To return borrowed item(s)

As seen in the below screenshot, this page uses an 'user interface' human coach. This page is provided to the user on login and the user performs an action of selecting one of the two above listed operations on this page.

The human interface attached to this activity is designed as shown in the screenshot:

![http://i.imgur.com/isdxAuq.jpg](http://i.imgur.com/isdxAuq.jpg)

This page also controls the level of accessibility of the above two listed items.
i.e, if the user is blocked, then the user is not allowed to borrow items.
The user can borrow items only if he is not blocked by the librarian.

Note: The user can be blocked, when he fails to return the book within the overdue period fixed by the university library management.

This action is controlled in a general system service "uOttawa Library Get User Status". This service calls  a stored procedure: sp\_GetUserStatus, which will return the status of the user(blocked/unblocked) from the Lib\_User table.

![http://i.imgur.com/4nHyGeL.jpg](http://i.imgur.com/4nHyGeL.jpg)

![http://i.imgur.com/a6bAxKu.jpg](http://i.imgur.com/a6bAxKu.jpg)

The variables created for this activity is shown in the screenshot:

![http://i.imgur.com/eZPRj5s.jpg](http://i.imgur.com/eZPRj5s.jpg)


The page looks like the following screenshot to the user:

![http://i.imgur.com/RAs4uvO.jpg](http://i.imgur.com/RAs4uvO.jpg)
As seen above, the coach displays a welcome message to the user:
"Hello UserName" and lets the user select one of the two options: Borrow/Return.

If the user is a blocked user, then a suitable message is displayed to the user as seen in the screenshot:
![http://i.imgur.com/DiWzUIK.jpg](http://i.imgur.com/DiWzUIK.jpg)