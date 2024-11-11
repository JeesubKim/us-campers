# Project: us-campers

Camping ticket P2P trading system

# Description

Hard to find the people who wants to cancel their reservation and hand over it.

This web site is to relay the people who want to purchase and who want to sell.

# Stack
- MSA architecture using docker and k8s
- Fast API for API server
- NATS for event bus
- mongodb for db
- redis for caching order and expire it!

# Resources
## user

## ticket

## order

## payment

# Services

## auth
User related service

## tickets
CRUD of Camping tickets

## orders
CRUD of order

## expiration
watches for orders to be created, cancels them after certain period times (30min)

## payments
handles credit card payments. Cancels orders if payment fails, completes if payment succeeds


# events

## User

- UserCreated
- UserUpdated

## Order

- OrderCreated
- OrderCancelled
- OrderExpired

## Ticket

- TicketCreated
- TicketUpdated

## ChargeCreated

- ChargeCreated
