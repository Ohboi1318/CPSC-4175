### CPSC 4175 - Homework 4 - Tristan Porter ###

#### 1. What is an entity class? A boundary class? A control class? ####

- An entity class is the information and associated behavior of some phenomenon or concepts such as an individual, a real life object, or a real life event.
- A boundary class is the terminus between the user and the system, or the system and other systems that it relies on.
- A control class represents co-ordination sequencing, transactions and control of other objects.

#### 2. Write a use case pertaining to your project. ####

User logs into system and the system recognizes their credentials and loads their account information. User clicks on an item and the system retrieves and displays the information related to that item. User adds the item to their shopping cart and checks out, the system totals the cost of the shopping cart and shows the user the total and asks for payment information. User inputs their payment method and the system recognizes and approves the transaction. The system logs this and notifies the company to send the item to the user.

#### 3. Write a successful scenario pertaining to your project. ####

A new user creates an account. They add a textbook to their shopping cart and click on checkout. They are shown the total cost and enter their payment information. This information is stored for later use and convenience. The transaction is approved and the textbook is shipped to the user using their preferred shipping method.

#### 4. Write an unsuccessful scenario pertaining to your project. ####

A returning user logs in and their shopping cart is not how they previously saved it. At some point all of their preferences and payment information have been deleted. However, they do not realize this until they proceed to checkout and they are unable to pay for the product. Or the shopping cart total is calculated incorrectly and the user is charged too much resulting in a lot of work on their part to fix it.

#### 5.  Using your answers to the three previous questions, use the noun extraction method to extract the classes. If practicable, identify the classes you extract as entity, boundary, and control classes. If all your classes are entity classes, you will not be able to do this. ####

- Entity classes - User; cart; order; item
- Boundary classes - Login/credentials; account
- Control classes - Transaction; Payment

#### 6. Using your answer to the previous question, draw an appropriate class diagram. ####

See attached document.

#### 7. Complete a CRC card for one of your classes. ####

See attached document.

#### 8. Draw a state chart for one specific behavior of your project. ####

See attached document.

#### 9. Draw a communication diagram for one specific realization of a use case. ####

See attached document.

#### 10. Draw a sequence diagram for one specific realization of a use case. ####

See attached document.

