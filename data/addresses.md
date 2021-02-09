# Addresses

> What are some interesting input tests for address validation?

## Kinds of Addresses
- Mailing or Shipping Address
    - Military Address
    - Post Office Box (PO Box)
    - Private Mailbox (PMB)
- Physical Address

### Not all mailing addresses are shipping addresses

Physical Address:
25777 Co Rd 103
Jelm, CO 82063

USPS Mailing Address:
25777 Co Rd 103
Jelm, WY 82063-9203

### Missing Street

Correct Address: 1200 Park Ave, Emeryville, CA 94608
Wrong Address: 1200 Park, Emeryville, CA 94608

### Wrong City

Correct Address: 1200 Park Ave, Emeryville, CA 94608
Wrong Address: 1200 Park Ave, Oakland, CA 94608

Correct Address: 2 Kirkland St, Cambridge MA 02138
Wrong Address: 2 Kirkland St, Boston MA 02138


### Wrong State

### Wrong Country


## Test Ideas

- Start with well known addresses that don't change
    - Hospitals
    - Schools / Universities
    - Cemeteries
    - Government Locations
    - Landmarks
-  