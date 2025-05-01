# airbnb-clone-project

The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security. This project enables learners to understand complex architectures, workflows, and collaborative team dynamics while building a scalable web application.

## Team roles

- **Product Owner:** A product owner is a decision maker, balancing both business needs and market trends, they define business strategy, shape up the product vision and make sure it satisfies customer needs. They will be responsible for making sure the `airbnb-clone-project` meet up with the requirement of the customers.
- **UI/UX Designer:** A UI/UX designer is a proffesional who focuses on desining digital products(like website, mobile apps) that are both user-friendly, visually appealing and easy to interact with interface. They will be responsible for designing the interfaces of the `airbnb-clone-project`.
- **Software Developer:** A software developer does the actual job and codes an application. There are front-end and backend developers.

  - **Front-end developers:** They create the part of an application that users interact with, ensuring that an app offers an equally smooth experience to all, no matter the devices, platform, or operating system. In the `airbnb-clone-project` they will be responsible for coding out the designs that the UI/UX Designer had workd on and also integrating the APIs.
  - **Backend developers:** They  implement the core of an app, its algorithms and business logic. Exprerienced backend developers not only write code but also do the tasks of an architect, for example, devise an app architecture or design and implement necessary integrations. They will be responsible for designing the database and exposing all necessary endpoints for the frontend developers to consume in the `airbnb-clone-project`.

- **Quality Assurancce:** The job of QA is to verify whether an application meets the requirement both functional and non-functional by running various checks. Their responsibility in the project will be to test out the functonality of the developed application by the software developers.

## Technology Stack

- **Django:** A high-level python web framework used for building the RESTful API.
- **Django REST Framework(DRF):** Provides tools for managing RESTful APIs.
- **PostgreSQL:** A powerful relational database use for data storage.
- **GraphQL:** Allows for flexible and effiecient querying for data.
- **Celery:** For handling asynchronous tasks such as sending notifications or processing payments.
- **Redis:** Used for caching and session management.
- **Docker:** Containerization tool for consistent development and deployment environment.
- **CI/CD Pipelines:** Automated pipelines for testing and deploying code changes.

## Database Design

### Key Entities

#### 1 Users

- `user_id`
- `email`
- `profile_picture`
- `prefers_email_notification`
- `roles`

#### 2 Properties

- `Property_id`
- `name`
- `property_type`
- `location`
- `availability`
- `price`

#### 3 Bookings

- `booking_id`
- `user`(foreign key -> Users)
- `property` (foreign key -> Properties)
- `start_at`
- `ends_at`
- `created_at`

#### 4 Reviews

- `review_id`
- `user`(foreign key -> Users)
- `property` (foreign key -> Properties)
- `review`
- `created_at`

#### 5 Payments

- `payment_id`
- `user`(foreign key -> Users)
- `property` (foreign key -> Properties)
- `payment_status`

### Relationships

- A  user can have multiple bookings
- A user can have many reviews
- A user can book many properties
- A booking belongs to a user and a property
- A review belong to a user and a property

## Feature Breakdown

- **API Documentations:** The backend API are documented to ensure clarity and ease of integration

- **User Authentcation:** Users must be able to register, authenticate and manage their profiles.

- **Property Management:** Implement creating, updating, retrieving and deleting of property listings.

- **Booking System:** Implement making, updating and management of bookings.

- **Payment Processing:** Handle payment transactions related to bookings.

- **Review System:** Post and manage reviews for properties.

- **Database Optimization**

  - **Indexing:** Implement indexes for fast retrieval of frequently accessed data.

  - **Caching:** Use caching strategies to reduce database load and improve perfomance.

## API Security

## CI/CD Pipeline

##