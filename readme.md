# Emaily - A React/Redux Email Survey App

This somewhat complex app was built for an online course taught by Stephen Grider: _Node with React: Fullstack Web Development_

---

**Description:**

The app flow is as follows:

1.  A user wants to send out a mass email to get feedback for their company's service/product. They visit the app URL.
2.  The visitor authenticates via a Google Auth page, and is returned to the app as a new user.
3.  The user adds tokens/credits to their account by clicking the 'add credits' button. A stripe payment pop-up collects money from the user.
4.  Once the payment processes (in a few seconds), the user is immediately credited to their account.
5.  User clicks the big '+' button to create a new survey. (This was kept basic for this app, but could easily be expanded. _e.g. mass import of email addresses via CSV file_)
6.  The survey details are confirmed, and then sent out via SendGrid's API. A credit is removed from the user's account.
7.  A webhook is running to catch event notifications from SendGrid. Clicks to the survey replies are stored in the (MongoDB) database for the appropriate survey and recipient. (Other info could also be tracked, such as bounces and opens.)
8.  The creator of the survey can view response tallies for their survey(s) at any time via the app dashboard.

---

**Features:**

* Custom Node.js / Express.js API backend
* React / Redux frontend
* Google OAuth authentication
* Stripe API payments
* MongoDB data storage (with Mongoose)
* SendGrid API for mass emails and click tracking
* "Wizard" style form for creating surveys
* Basic stying via Materialize CSS

---

**Notes:**

* Styling was kept SUPER minimal for this app. The focus was on functionality!

* SendGrid's free accounts are only good for 30 days, so this will app not have a preview/demo link available.

* To test out the demo, you wll need a Stripe (developer) account and a SendGrid account. You'll also need a Google+ OAuth API key.

* I definitely learned a TON from this course! My overall React/Redux comfort levels increased dramatically, as well as my general ES6 JavaScript knowledge. I'm really looking forward to expanding upon this material and creating some interesting things in the near future!





# Emaily - Simple Feedback Collection Service

Emaily is a MERN full-stack web application that allows users to send mass emails to a large list of users for the purpose of collecting feedback. It has an authentication system implemented using Passport.js and Google Oauth and provides functional billing and payment processing using the Stripe API. It uses Mongoose for survey creation and utilizes the SendGrid API to automatically send emails to recipients.

<strong>Emaily live link:</strong> https://orm-emaily.herokuapp.com/

<img width="1279" alt="landing-screenshot" src="https://prnt.sc/qjly5t">

## Technologies and Frameworks Used

* <strong>Front-end:</strong> React.js, Materialize.css
* <strong>Back-end:</strong> Node.js, Express, MongoDB
* <strong>Deployment:</strong> Heroku
* <strong>Authentication:</strong> Passport, OAuth 2.0

