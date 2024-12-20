# legacy-book-store

# Contributors
* [Sebastien Noirot](https://github.com/seb-noirot) 

# Use Cases
1. **Browse Books**: Users can browse through a list of available books.
2. **Search Books**: Users can search for books by title, author, or genre.
3. **View Book Details**: Users can view detailed information about a book, including its description, author, and price.
4. **Add to Cart**: Users can add books to their shopping cart.
5. **Checkout**: Users can purchase the books in their shopping cart.
6. **User Registration and Login**: Users can create an account and log in to access their personal information and order history.
7. **Order History**: Users can view their past orders and order details.
8. **Leave Reviews**: Users can leave reviews and ratings for books they have purchased.

# External Systems
* External I/O System: jsonplaceholder (https://jsonplaceholder.typicode.com/)
* External Non-deterministic System: System Clock

# System Architecture Style
The chosen architecture for this system is "Frontend + Monolithic Backend".

# Architecture Diagram
```
+-----------+          +-----------+
| Frontend  | <------> |  Backend  |
+-----------+          +-----------+
      |                      |
      v                      v
+----------------+    +----------------+
| jsonplaceholder|    |  System Clock  |
+----------------+    +----------------+
```

# Tech Stack
* Programming Language: Java, Javascript
* Frameworks: Quarkus, React
* Database: MySQL
* Message Broker: Kafka
* Other Technologies: Docker, Maven

# Repository Strategy
The chosen repository strategy for this project is the Mono-Repo approach. All components of the system are maintained in a single repository. This approach allows for easier management of dependencies, centralized version control, and simplified development and testing of the entire system.

# Branching Strategy
The chosen branching strategy for this project is Feature Branching. Each new feature or bug fix is developed in its own branch, which is then merged into the main branch after review and approval.

# Deployment Model
We chose Google Cloud Platform (GCP) as our deployment model. 
