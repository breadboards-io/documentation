# How to use the style editor


The Style Editor is located on the right side panel and is used to style UI elements from scratch or modify imported components. Breadboard makes it easy to swap, move, and scale elements using either free-form placement or structured auto-layouts, ensuring your interface remains organized and functional.


#### 💡 Pro-Tip for Figma Users
To import your designs, use the Figma to Code plugin. This ensures that your Figma Auto-Layout settings—including spacing, buttons, and containers—are transferred exactly as designed and maintain the same behavior in Breadboard.


### Attributes
<img src="https://cdn.breadboards.app/assets/documentation/03_Style editor_1.png">
Selecting a UI element displays its properties at the top of the Style Editor. Here, you can rename the element or change its type – for example, switching an element from a Container to a Text or Input field –.


### Positions
<img src="https://cdn.breadboards.app/assets/documentation/03_Style editor_2.png">
The Position property determines whether an element participates in the screen's Document Flow — the system that automatically arranges elements—or ignores it to be placed independently. Breadboard uses CSS position rules to ensure your design remains fully responsive, allowing you to use X (Left) and Y (Top) coordinates for precise placement.


#### In-Flow
Elements that are "In-Flow" occupy physical space and influence the position of the elements around them.

- <img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_1.png"> **Static**: The default setting. Elements follow the natural order of the layout and cannot be manually shifted.
- <img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_2.png"> **Relative**: The element stays in the normal flow, but you can use **X (Left)** and **Y (Top)** to shift its appearance without affecting the space it originally occupied.
- <img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_3.png"> **Sticky**: The element behaves like a Static element until it reaches a specific scroll point, where it then "sticks" to its position.


#### Out-of-Flow
Elements that are "In-Flow" occupy physical space and influence the position of the elements around them.

- <img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_4.png"> **Absolute**: The element is placed at a specific **X (Left)** and **Y (Top)** position relative to its parent container.
- <img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_5.png"> **Fixed**: The element is locked to a specific **X (Left)** and **Y (Top)** coordinate on the screen and remains in that spot even when the user scrolls.

