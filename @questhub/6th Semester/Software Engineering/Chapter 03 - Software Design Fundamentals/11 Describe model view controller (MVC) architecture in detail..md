---
class: cse
title: 11 Describe model view controller (MVC) architecture in detail.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-08-04
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2022
  - board_2018
aliases:
  - "Describe with diagram the process activities of MVC architecture. #board_2018"
---


### Process Activities of MVC Architecture

**MVC (Model-View-Controller)** is a software design and architectural pattern that divides an application into three interconnected components: **Model, View, and Controller**. This separation ensures that data management, user interface, and input handling are independent, which improves **modularity, maintainability, scalability, and ease of development**.

---

### Components of MVC

- **Model**  
    The **Model** represents the data and business logic of the application. It manages application state, performs data processing, applies rules, and communicates with databases or external resources. The Model is independent of the user interface, allowing it to be reused across different Views.
    
- **View**  
    The **View** is responsible for displaying information to the user. It presents data from the Model in a readable format, such as web pages, forms, or charts. The View does not handle business logic; it only observes the Model and renders the output.
    
- **Controller**  
    The **Controller** acts as an intermediary between the View and the Model. It receives input from the user via the View, interprets it, and decides how the Model should be updated. It also determines which View should be displayed in response to user actions.
    

---

### Process Activities

- **User Interaction**  
    The user interacts with the **View** by performing actions such as clicking buttons, entering data in forms, or navigating through menus. This step initiates the flow of control in the system.
    
- **Controller Receives Input**  
    The **Controller** captures the user input from the View and interprets it to determine what action should be taken. It acts as an intermediary between the View and the Model, ensuring proper handling of requests.
    
- **Controller Updates Model**  
    Based on the user input, the Controller requests the **Model** to perform operations such as updating data, applying business logic, or retrieving information. The Controller does not handle data processing directly, keeping responsibilities separated.
    
- **Model Processes Data**  
    The **Model** executes the necessary operations, validates inputs, applies business rules, and updates its internal state. It may also trigger notifications to the View about changes so the interface can reflect updated data.
    
- **View Updates Output**  
    The **View** retrieves updated data from the Model and refreshes the user interface accordingly. This ensures that the user always sees the latest information and the system’s response to their actions.
    
- **Feedback to User**  
    The updated View presents results to the user, providing feedback on their actions. The user can then continue interacting with the system, which restarts the MVC cycle.

![[Working-of-MVC-1024x686.png]]


---

### Advantages of MVC

- **Separation of Concerns** – Each component (Model, View, Controller) has a distinct responsibility, reducing complexity and making the system easier to manage.    
- **Reusability** – Models and Views can be reused across different parts of the application or in other projects.    
- **Maintainability** – Changes in one component (e.g., updating the user interface) have minimal impact on others.    
- **Parallel Development** – Developers can work simultaneously on the Model, View, and Controller without interfering with each other.    
- **Improved Testability** – Business logic is separated from the interface, making it easier to test the Model independently.    
- **Flexibility** – Multiple Views can represent the same data in different ways, enhancing user experience.