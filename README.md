# TrenchCoat-Boutique

### Description

Trench coats are cool. Everyone should own a trench coat. The *“Proper Trench Coats”* store sells fashionable, elegant trench coats and the store needs software to allow their customers to order online. The application can be used in two modes: administrator and user. When the application is started, it will offer the option to choose the mode.
**Administrator mode:** The application will have a database which holds available trench coats at a given moment. The store employees must be able to update the database, meaning: add a new trench coat, delete a trench coat (when it is sold out) and update the information of a trench coat. Each **Trench Coat** has a `size`, a `colour`, a `price`, a `quantity` and a `photograph`. The photograph is memorised as a link towards an online resource (the photograph on the presentation site of the store). The administrators will also have the option to see all the trench coats in the store.\
**User mode:** A user can access the application and choose one or more trench coats to buy. The application will allow the user to:
- See the trench coats in the database, having a given size, one by one. When the user chooses this option, the data of the first trench coat (size, colour, price, quantity).
- Choose to add the trench to the shopping basket. In this case, the price is added to the total sum the user has to pay.
- Choose not to add the trench coat to the basket and to continue to the next. In this case, the information corresponding to the next trench coat is shown and the user is again offered the possibility to buy it. This can continue as long as the user wants, as when arriving to the end of the list, if the user chooses next, the application will again show the first trench coat.
- Display the current trench coat.
- See the shopping basket and the total price of the items.
- Display the shopping basket in a CSV or HTML file, depending of the option the user selected.

<br><br>

### Details
  - The application is implemented using **Layered Arhitecture** (domain, repository, controller/service, gui)
  - The UML Diagram of the project can be visualized by accessing `diagram.svg`.
  - The repository is loaded automatically from file `initRepository.txt` at the beggining of the application. Any changes done to the repository during the runtime are saved in the same file.
  - The basket is implemented using **Polymorphism**. An abstract basket is instantiated at the beggining of the program and depending of the user option it can be set to an **HTML** or **CSV** basket, such the user is able to open the basket file in the correct format.
  - Validations and Custom exception classes for Trench Coat and Repository exceptions are used.
 
 <br><br>

 ### Show case
 
![start window](https://user-images.githubusercontent.com/9745845/236486916-2b2067a9-230e-4bcd-b7d7-702a6ece3375.PNG)

![admin window](https://user-images.githubusercontent.com/9745845/236486949-b3998958-bf59-483a-84d6-93bb5c62c5aa.PNG)

![user window](https://user-images.githubusercontent.com/9745845/236486953-43578e10-b2e3-4ac3-8385-ee89f6a58aba.PNG)

<br><br>
### Project Setup Recommandation:
  - install Visual Studio.
  - install QT Framework.
  - link Visual Studio with QT 5.
  - setup a new QT Widget Application C++ project in Visual Studio.
  - copy all the files from `Project` directory in the new created project.
  - run the program. 
