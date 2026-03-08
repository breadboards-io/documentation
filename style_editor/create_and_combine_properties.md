# Components & Instances

<img src="https://cdn.breadboards.app/assets/documentation/04_Components & instances_1.png">

In Breadboard, Components and Instances represent the relationship between a Main Component and its Instances. This system allows you to define a UI element once and reuse it across multiple screens, ensuring interface consistency and eliminating the need to recreate the same elements repeatedly.

### The Main Component 
**Definition**: A reusable, self-contained UI element that serves as the **Single Source of Truth**.

- **Role** : It defines the layout, appearance, and behavior of a specific element, such as a Button, Navigation Bar, or Card.
- **Behavior** : Any change made to the Main Component is automatically updated in every instance across your entire project.


### The Instance 
**Definition**: A specific occurrence of a Component placed within a layout.

- **Role** : It acts as a reference to the Main Component, automatically inheriting all of its layout, styling, and behavior.
- **Behavior** : Instances stay synchronized with the Main Component. If you update the Main Component, the changes are automatically applied to all its instances. Once you connect properties, it’s possible to override the component content and/or style. You can learn more about the ‘Create and connect properties’ section.


### Summary Table
| **Feature**      | **Main Component**                         | **Instance**                                   |
|------------------|--------------------------------------------|------------------------------------------------|
| **Purpose**      | To define the design and rules             | To use the design in context                   |
| **Editing**      | Changes update **every instance** globally | Changes affect **only that specific instance** |
| **Relationship** | The Parent / Blueprint                     | The Child / Implementation                     |
