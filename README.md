
# MEAN (server : Nest.js with Mongoose, client : Angular, server-ssr : Server-side rendering - build both)




## Description
- eShop-MeanStack with products and administration
- Typescript stack with decorators, use MongoDB and mongoose schemas, JWT Passport

## Installation

One package.json contain now all neccessary for Nest and Angular, so server-side rendering with Angular is possible

```bash
$ npm install
```

## Running the app

```bash
# development - start BE - port 4000
$ npm run start

# development - start FE - port 3000
$ npm run start:client

# watch mode server
$ npm run start:dev

# build ssr, watch for changes doesnt work well now
$ npm run dev:ssr

# build ssr and serve
$ npm run build:ssr
$ npm run serve:ssr
```

For another commands look to package.json

## SET ENVIROMENT FOR BE - Rename .env.example to .env

```bash
# BE HOST
SERVER_PORT=4000
SERVER_URL="http://localhost:4000"

# FE HOST
ORIGIN="http://localhost:3000"

# JWT settings
JWT_EXPIRATION="7d"
JWT_SECRET="youhavetochoseone"

COOKIE_KEY="youhavetochoseone"

# DB URI
MONGO_URI="mongodb://{user}:{password}@{host}:{port}/{databaseName}"

# Emails
SENDGRID_KEY="set if you want have notification for order or contact from https://sendgrid.com (ADMIN_EMAILS and user will get notification)"

# Images
CLOUDINARY_NAME="set name from cloudinary api https://cloudinary.com (for images upload)"
CLOUDINARY_KEY="set key from cloudinary api  https://cloudinary.com (for images upload)"
CLOUDINARY_SECRET="set secret from cloudinary api https://cloudinary.com (for images upload)"

# Pay
STRIPE_PUBLISHABLE_KEY="set for paying with card for orders with stripe https://stripe.com"
STRIPE_SECRETKEY="set for paying with card for orders with stripe https://stripe.com"

# Google login
GOOGLE_CLIENT_ID="set for google login activation"
GOOGLE_CLIENT_SECRET="set for google login activation"

# Admin emails get notification from sendgrid when order or contact are submitted
ADMIN_EMAILS="your@email.com, another@mail.com"

RECAPTCHA_SERVER_KEY="RECAPTCHA_SERVER_KEY"

# FE ENV SEND FROM BE
FE_STRIPE_PUBLISHABLE_KEY="FE_STRIPE_PUBLISHABLE_KEY"
FE_TINYMCE_API_KEY="FE_TINYMCE_API_KEY"
FE_RECAPTCHA_CLIENT_KEY="FE_RECAPTCHA_CLIENT_KEY"
```
