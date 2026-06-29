# 🛒 E-Commerce Ontology

**Knowledge Representation Exam Project**

**Student:** Finhas Demissie  
**Program:** Master's Degree in Artificial Intelligence  
**University:** University of Verona  
**Course:** Knowledge Representation  
**Ontology Language:** OWL 2.0  
**Development Tool:** Protégé 5.6.9  
**Reasoner:** HermiT

---

# 📖 Project Description

This project presents an **E-Commerce Ontology** developed in **OWL 2.0** using **Protégé**.

The ontology models the knowledge of an online shopping platform by representing customers, sellers, products, shopping carts, orders, payments, shipments, reviews, and addresses, together with the semantic relationships among them.

The ontology has been validated using the **HermiT Reasoner**, ensuring that it is logically consistent.

---

# 🎯 Objectives

The ontology aims to:

- Represent an online shopping environment.
- Model semantic relationships between entities.
- Support logical reasoning over e-commerce knowledge.
- Demonstrate ontology engineering using OWL 2.0.

---

# 🏗 Ontology Structure

## Main Classes

```
Thing
│
├── Person
│   ├── Customer
│   └── Seller
│
├── Product
│   ├── Electronics
│   │   ├── Smartphone
│   │   ├── Laptop
│   │   └── Tablet
│   │
│   ├── Clothing
│   │   ├── MenClothing
│   │   ├── WomenClothing
│   │   └── KidsClothing
│   │
│   ├── Book
│   │   ├── PrintedBook
│   │   └── EBook
│   │
│   └── Accessory
│       ├── Keyboard
│       ├── Mouse
│       └── Headphones
│
├── ShoppingCart
├── Order
├── Payment
├── Shipment
├── Review
└── Address
```

---

# 🔗 Object Properties

| Property | Domain | Range |
|----------|---------|--------|
| hasShoppingCart | Customer | ShoppingCart |
| placesOrder | Customer | Order |
| containsProduct | Order | Product |
| containsItem | ShoppingCart | Product |
| hasPayment | Order | Payment |
| hasShipment | Order | Shipment |
| hasAddress | Customer | Address |
| writesReview | Customer | Review |
| reviewsProduct | Review | Product |
| sells | Seller | Product |

---

# 📝 Data Properties

### Customer

- hasCustomerName
- hasEmail
- hasPhoneNumber

### Product

- hasProductName
- hasPrice
- hasStockQuantity

### Order

- hasOrderDate

### Payment

- hasPaymentMethod
- hasPaymentStatus

### Shipment

- hasShipmentStatus
- hasTrackingNumber

### Review

- hasRating
- hasComment

---

# 👥 Example Individuals

## Customers

- AliceJohnson
- BobSmith
- CharlieBrown

## Sellers

- TechStore
- FashionHub
- BookWorld

## Products

### Electronics

- iPhone15
- DellXPS13
- iPadAir

### Accessories

- MechanicalKeyboard
- LogitechMouse
- SonyHeadphones

### Clothing

- BlueTShirt
- WomenDress
- KidsJacket

### Books

- AIBook
- OWLGuide

## Shopping Carts

- Cart001
- Cart002
- Cart003

## Orders

- Order001
- Order002
- Order003

## Payments

- Payment001
- Payment002
- Payment003

## Shipments

- Shipment001
- Shipment002
- Shipment003

## Reviews

- Review001
- Review002
- Review003

## Addresses

- AddressAlice
- AddressBob
- AddressCharlie

---

# 🧠 Reasoning

The ontology was verified using the **HermiT Reasoner**.

✔ No logical inconsistencies were detected.

✔ All classes and individuals were correctly classified.

---

# 📂 Repository Structure

```
EcommerceOntology
│
├── EcommerceOntology.ttl
├── README.md
├── OntologyGraph.png
└── (optional) EcommerceOntology.owl
```

---

# 🚀 How to Use

1. Install **Protégé 5.6.9** or later.
2. Open `EcommerceOntology.ttl`.
3. Start the **HermiT Reasoner**.
4. Explore:
   - Classes
   - Object Properties
   - Data Properties
   - Individuals
   - OntoGraf

---

# 🛠 Technologies Used

- OWL 2.0
- Protégé 5.6.9
- HermiT Reasoner
- OntoGraf

---

# 👨‍🎓 Author

**Finhas Demissie**

Master's Degree in Artificial Intelligence

University of Verona

Academic Year 2025–2026

---

# 📜 License

This project was developed solely for academic purposes as part of the **Knowledge Representation** course at the **University of Verona**.
