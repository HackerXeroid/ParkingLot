## Multi-Level Parking Lot System

This document outlines the design considerations and functionalities for a multi-level parking lot system.

### User Stories (User Journey)

* A user can create a parking ticket upon entering the lot.
* The system assigns a parking spot based on vehicle size and availability.
* The user pays for parking upon exiting the lot.

### System Visualization (Physical Structure)

The system consists of the following:

* **Parking Lot:**
    * **Floors (Multiple):** Each floor has entry/exit gates with operators.
    * **Parking Spots (Multiple per Floor):** Spots are categorized by size (Small, Medium, Large). Some spots are designated for Electric Vehicles (EV) with charging stations (available/under maintenance status).
* **Database:** Stores user, vehicle, ticket, and payment information.

### System Requirements

**Entities:**

* **Ticket:** Represents a parking session with details like entry time, assigned spot, and fees.
* **Bill:** Generated upon exit, showing total parking charges.
* **User:** Creates parking tickets and makes payments.
* **Parking Spot:** Represents a designated parking space with size and EV charging facility information.

**Functionalities:**

* **Ticket Generation:** Creates a ticket upon vehicle entry.
* **Parking Spot Assignment:** Assigns a suitable parking spot based on vehicle size and availability.
* **Bill Generation:** Calculates and generates a bill upon vehicle exit.
* **Payment Processing:** Handles different payment modes (full or partial payments).
* **Vehicle Details Storage:** Stores information about the parked vehicle.
* **Entry/Exit Gate Management:** Tracks vehicle entry and exit with operator assistance.

**Additional Considerations:**

* **Incremental Billing:** Applies charges based on time intervals (e.g., every 2 hours at the airport).
* **Multiple Payment Modes:** Accepts various payment options for user convenience.
* **Owner Details:** Stores owner information for future reference (optional).


**Next Steps:**

* Develop detailed API specifications.
* Design database schema.
* Implement core functionalities.

This document provides a high-level overview of the system requirements. Further refinement and detailed design will be necessary during development.
