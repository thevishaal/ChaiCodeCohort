# Comic-Con Parking System (ERD Design)

## Overview 

This assignment presents the **ERD** design for a large-scale **multi-zone parking management system**.

The system is designed to efficiently handle thousands of vehicles entering and exiting the venue across multiple days, while supporting:

- Different vehicle types (bike, car, SUV, EV, cab)
- Reserved parking categories (VIP, exhibitors, staff, cosplayers)
- Multi-level parking zones
- Ticket generation and session tracking
Payment processing

## Objectives 

The ERD is designed to answer the following:

- Track all vehicles entering the parking facility
- Identify vehicle types
- Allocate appropriate parking spots
- Manage reserved parking categories
- Record entry and exit timestamps
- Track active and completed parking sessions
- Calculate and store parking charges
- Maintain payment records
- Monitor parking availability in real-time

## Entities

- vehicle  
- vehicle_category  
- parking_zone  
- parking_spot
- parking_spot_category
- parking_ticket
- parking_session
- payment
- pricing_rule

## Relationships

vehicle → parking_session → One-to-Many  
parking_spot → parking_session → One-to-Many  
parking_zone → parking_spot → One-to-Many  
parking_spot_category → parking_spot → One-to-Many  
vehicle_category → vehicle → One-to-Many   
parking_session → parking_ticket → One-to-One   
parking_session → payment → One-to-One

## Notes

- Primary Keys (PK) and Foreign Keys (FK) are clearly defined in the diagram.
- The design follows normalization principles to avoid redundancy.


## Feedback is most welcome