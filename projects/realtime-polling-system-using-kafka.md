# Real-Time Polling System (Kafka-based)

## Description
A real-time polling application that allows users to vote and see live results instantly. The system is built using Kafka for event-driven architecture to handle high-throughput voting.

## Features
- Real-time vote processing using Kafka
- Instant live poll results update
- Scalable architecture for high user load
- Secure vote storage and fraud detection mechanisms
- Web-based interactive dashboard for viewing poll results

## Technologies Used
- **Backend:** Node.js
- **Event Streaming:** Kafka
- **Frontend:** React.js
- **Database:** PostgreSQL

## Challenges Faced & Solutions
- **Issue:** Handling concurrent voting at scale
  - **Solution:** Used Kafka to distribute events and process votes in parallel
- **Issue:** Preventing duplicate or fraudulent votes
  - **Solution:** Implemented unique user authentication and validation checks