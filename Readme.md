Global pass project

Global pass

User

1. View services
2. Select service
    1. University application
    2. Udemy or any course
    3. Subscription Ai tools, Netflix etc..
    4. Hotel booking
    5. Exam fee
3. Book service with requirements
    1. Service name
    2. Login link, with user name password
    3. Amount
    4. Currency
    5. Description on steps to follow
    6. Any more detailed information required
4. View booked services
5. View finalized services
6. Send Payment proof
7. Customer support page

Admin
1. View bookings
2. Select booking
3. Accept booking - > send notification via email and redirection to app
4. Reject booking with information -> send notification
5. Send proof of payment
6. View users - with their bookings


Backend APIs (MVP)
Auth
POST /auth/register
POST /auth/login
GET /auth/me

Services
GET /services
GET /services/:id
Orders (Main Core)
POST /orders
GET /orders
GET /orders/:id

Forex
GET /exchange-rate
POST /orders/calculate-price
Payments
POST /payments
GET /payments/:id

Admin
GET /admin/orders
PATCH /admin/orders/:id/accept
PATCH /admin/orders/:id/reject
PATCH /admin/orders/:id/complete
POST /admin/orders/:id/proof

Users (Admin)
GET /admin/users

Option 1 (Best)
Build:
POST /orders
GET /orders
Option 2

Design database tables:-
users
orders
payments
services
