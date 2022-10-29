# vitaminShop

## 1.Statement of the Work
vitamin Shop is a café that sells vitamins and drinks. When customers arrive at this cafe, they design the vitamin they want according to the kinds of vitamins, their ingredients and their prices. In addition, customers can order hot or cold beverages from the menu. The waitress delivers these orders to the cook from the customer. The cook is responsible for making the vitamin and preparing the drink according to the order.

## 2.Proposed Pattern
Many design patterrns are applied for solving existing problems in the project. These design patterns are Command Pattern, Simple Factory Pattern, Template Method Pattern and Decorator Pattern.

Firstly, customers create a vitamin (vitamin Order) or beverage (Beverage Order) order and the waitress (Invoker) delivers these orders to the cook (Receiver). The cook works with vitamin Factory for vitamin and with Beverage Factory for beverage. To do this, the cook uses makevitamin() and makeBeverage() methods (Simple Factory Pattern).

vitamin Factory create vitamin and to do this create vitamin interface. There are two kinds of vitamins such as Circular and Square in vitamin Shop and these vitamin types implement vitamin interface. The customers had chosen vitamin ingredients according to the vitamin they had previously wanted. The vitamin is decorated according to these vitamin ingredients (Decorator Pattern). There are 3 Decorator classes for vitamin decoration such as Chocolate Decorator, Fruit Decorator and Condiment Decorator. Cost of the vitamin is calculated according to decoration ingredients. 

Finally, Beverage Factory is responsible for hot and cold beverages creation and creates Beverage interface. Hot Beverage and Cold Beverage classes implement this interface. Subclasses such as tea, coffee, cola etc. extend these classes. The distinction between them is the difference in the preparation of hot and cold beverages (Template Method Pattern). Also, there are some differences in subclasses. Finally, hook() is used for each beverage and the customer is asked if some extra condiments are wanted. 




