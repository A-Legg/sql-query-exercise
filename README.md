# SQL Exercise

Let's write some SQL!

In this exercise we are going to practice writing SQL against an e-commerce database.

We will be working with four tables: customers, items, orders, and orderitems.

**customers**

    Column   |  Type   |                       Modifiers
    ---------+---------+--------------------------------------------------------
     id      | integer | not null default nextval('customers_id_seq'::regclass)
     name    | text    |
     email   | text    |
     address | text    |
     city    | text    |
     state   | text    |
     zipcode | text    |

**items**

     Column      |  Type   |                     Modifiers
    -------------+---------+----------------------------------------------------
     id          | integer | not null default nextval('items_id_seq'::regclass)
     name        | text    |
     description | text    |

**orders**

     Column      |  Type   |                      Modifiers
    -------------+---------+-----------------------------------------------------
     id          | integer | not null default nextval('orders_id_seq'::regclass)
     customer_id | integer |
     amount      | numeric |

 **orderitems**

       Column  |  Type   |                        Modifiers
     ----------+---------+---------------------------------------------------------
      id       | integer | not null default nextval('orderitems_id_seq'::regclass)
      order_id | integer |
      item_id  | integer |

# Setup

1. Fork and clone this repository
1. Import the Tracker stories in `stories.csv`
