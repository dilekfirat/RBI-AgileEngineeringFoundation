# US4200 - Additional Delivery options 

## Background
In the current version following deliver options and pricing are implemented:
| Option (`delivery_method`) | USD (billing country ≠ CZ) | CZK (billing country = CZ) |
|----------------------------|----------------------------|----------------------------|
| `standard`                 | $4.99                      | 99 Kč                      |
| `zasilkova`                | $1.99                      | 49 Kč                      |

Pricing is flat and does not consider shipping region or order weight.

## User story

**As a** shop owner  
**I want** additional delivery options to be available and delivery costs to be calculated from the selected delivery option, shipping region, and order weight  
**So that** the user can save costs for an order.

## New Delivery Options

### Weight tiers
Delivery cost depends on the **total order weight** (sum of all cart line items):

| Tier   | Condition        |
|--------|------------------|
| Light  | total weight < 10 kg  |
| Heavy  | total weight ≥ 10 kg  |

### Regional availability

| Option (`delivery_method`) | Available shipping regions |
|----------------------------|----------------------------|
| `standard`                 | CZ, EU, US, Others         |
| `zasilkova`                | CZ, DACH only              |

**Region definitions**

| Region  | Shipping countries |
|---------|--------------------|
| CZ      | Czech Republic     |
| DACH    | Germany, Austria, Switzerland |
| EU      | European Union member states except CZ |
| US      | United States      |
| Others  | All countries not listed above |

**Rules**
- `standard` is offered for every shipping destination (mapped to one of the four regions).
- `zasilkova` is offered only when the shipping country is in **CZ** or **DACH**; it must not appear for EU (non-DACH), US, or Others destinations.
- Currency display follows billing country: **CZK** when billing country = CZ, otherwise **USD**.

### Pricing — Standard (`standard`)

| Region | Weight   | USD (billing country ≠ CZ) | CZK (billing country = CZ) |
|--------|----------|----------------------------|----------------------------|
| CZ     | Light    | $2.99                      | 59 Kč                      |
| CZ     | Heavy    | $5.99                      | 119 Kč                     |
| EU     | Light    | $4.99                      | 99 Kč                      |
| EU     | Heavy    | $9.99                      | 199 Kč                     |
| US     | Light    | $6.99                      | 139 Kč                     |
| US     | Heavy    | $12.99                     | 259 Kč                     |
| Others | Light    | $8.99                      | 179 Kč                     |
| Others | Heavy    | $15.99                     | 319 Kč                     |

### Pricing — Zásilkovna (`zasilkova`)

| Region | Weight   | USD (billing country ≠ CZ) | CZK (billing country = CZ) |
|--------|----------|----------------------------|----------------------------|
| CZ     | Light    | $1.99                      | 49 Kč                      |
| CZ     | Heavy    | $3.99                      | 79 Kč                      |
| DACH   | Light    | $2.49                      | 59 Kč                      |
| DACH   | Heavy    | $4.99                      | 99 Kč                      |

## Acceptance criteria

- ACC-01: Checkout shows `standard` for shipping addresses in CZ, EU, US, and Others.
- ACC-02: Checkout shows `zasilkova` only for shipping addresses in CZ and DACH (DE, AT, CH).
- ACC-03: `zasilkova` is not shown for EU (non-DACH), US, or Others shipping destinations.
- ACC-04: Delivery cost uses the Light tier when total order weight is below 10 kg.
- ACC-05: Delivery cost uses the Heavy tier when total order weight is 10 kg or more.
- ACC-06: The displayed delivery price matches the matrix for the selected option, region, weight tier, and billing currency.
