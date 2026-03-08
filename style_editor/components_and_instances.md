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


### How to create components & instances
<video src="https://cdn.breadboards.app/assets/documentation/04_Components & instances_2.mp4" controls="" autoplay=""></video>
To create a master component simply click on a target element and click on the component icon from the contextual menu on top of it. Once the component is created, it is created on canvas, wrapped in a purple box.

<img src="https://cdn.breadboards.app/assets/documentation/04_Components & instances_3.png">
You can also add more variants of components by clicking on + under the “variants” badge.

<video src="https://cdn.breadboards.app/assets/documentation/04_Components & instances_4.mp4" controls="" autoplay=""></video>
<video src="https://cdn.breadboards.app/assets/documentation/04_Components & instances_5.mp4" controls="" autoplay=""></video>
After creating a component and its variant(s), simply copy the variant from the component group and paste it to the desirable location. You can also use the dock UI > Container > Custom component menu to add an instance of the component to the screen design. 


### Connect properties to component
<img src="https://cdn.breadboards.app/assets/documentation/04_Components & instances_6.png">

To combine properties that you created to a certain component, click on the target component and tap “combine properties”. Here, you can tie properties to its sub UI elements. To learn more about properties, check **Create & Combine Properties** 

