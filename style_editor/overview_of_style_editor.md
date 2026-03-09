# How to use the style editor


The Style Editor is located on the right side panel and is used to style UI elements from scratch or modify imported components. Breadboard makes it easy to swap, move, and scale elements using either free-form placement or structured auto-layouts, ensuring your interface remains organized and functional.


#### 💡 Pro-Tip for Figma Users
To import your designs, use the Figma to Code plugin. This ensures that your Figma Auto-Layout settings—including spacing, buttons, and containers—are transferred exactly as designed and maintain the same behavior in Breadboard.


### Attributes
<img src="https://cdn.breadboards.app/assets/documentation/03_Style editor_1.png">
Selecting a UI element displays its properties at the top of the Style Editor. Here, you can rename the element or change its type – for example, switching an element from a Container to a Text or Input field –.


### Positions
<img src="https://cdn.breadboards.app/assets/documentation/03_Style editor_2.png">
The **Position** property determins whether an element participates in the screen's **Document Flow** - the system that automatically arranges elements— or ignores it to be placed independently. Breadboard uses CSS position rules to ensure your design remains fully responsive, allowing you to use **X(Left) and Y(Top)** coordinates for precise placement.

#### In-Flow
Elements that are "In-Flow" occupy physical space and influence the position of the elements around them.

<ul class="list--image">
  <li><img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_1.png"><p>**Static**: The default setting. Elements follow the natural order of the layout and cannot be manually shifted.</p></li>
  <li><img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_2.png"><p>**Relative**: The element stays in the normal flow, but you can use **X (Left)** and **Y (Top)** to shift its appearance without affecting the space it originally occupied.</p></li>
  <li><img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_3.png"><p>**Sticky**: The element behaves like a Static element until it reaches a specific scroll point, where it then "sticks" to its position.</p></li>
</ul>


#### Out-of-Flow
Elements that are "Out-of-Flow" are removed from the standard layout. They do not take up space, meaning other elements behave as if they aren't there, which allows for overlapping content.

<ul class="list--image">
  <li><img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_4.png"><p>**Absolute**: The element is placed at a specific **X(Left)** and **Y(Top)** position relative to its parent container.</p></li>
  <li><img width="32" height="32" src="https://cdn.breadboards.app/assets/documentation/03_Style editor_3_5.png"><p>**Fixed**: The element is locked to a specific **X(Left)** and **Y(Top)** coordinate on the screen and remains in that spot even when the user scrolls.</p></li>
</ul>


#### Summary Table for Visualization
| **Position** | **Removed from Flow?** | **Reference Point (Coordinate Origin)**         | **Affects Surroundings?** |  
|--------------|------------------------|-------------------------------------------------|---------------------------|
| Static       | No                     | Preceding elements (Document Flow)              | Yes (Pushes others)       |   
| Relative     | No                     | Itself (Original Static Location)               | No (Space reserved)       |   
| Absolute     | Yes                    | Nearest Non-Static Ancestor                     | No (Others ignore it)     |   
| Fixed        | Yes                    | Viewport (Browser Window)                       | No (Others ignore it)     |   
| Sticky       | No                     | Itself -> then Viewport (constrained by Parent) | Yes (Space reserved)      |   


### Auto-layout (= ‘flex’ in CSS)
<img src="https://cdn.breadboards.app/assets/documentation/03_Style editor_4.png">

Auto Layout is a dynamic property that allows containers to automatically resize and rearrange their children based on the content inside. It is most commonly used in design tools like Figma, but in case you are not familiar with Figma and/or you have a technical background - originally it is best described as the visual interface for **CSS Flexbox**.

Instead of manually placing elements at fixed coordinates (like position: absolute), Auto Layout establishes a strict relationship between the parent container and its child items so it’s a lot easier for users to create a “format” of UI components or screen design efficiently.

It calculates the layout based on three factors:
- Direction: Item can be stacked horizontally (Row) or vertically (Column)
- Spacing: How much gap is between items and how much padding surrounds them?
- Sizing: You can determine the dimension either absolutely (ex. 360px) or relatively (ex. 100vw)
  
Auto layout removes the need for manual pixel-pushing, ensuring designs stay responsive when text changes or items are added/removed.


### Appearance
With the appearance menu, you can tweak a wide variety of visual attributes of the selected UI elements including: 

- **Opacity**: Transparency of an element 
- **Corner radius**: Makes all or each corner round
- **Scroll**: Gives scrollability on a selected screen
  - **Visible**: this is the default option - the screen overflow is NOT clipped
  - **Hidden**: the overflow is clipped, and the rest of the content is hidden
  - **Scroll**: scrollbars are added and users must scroll to see all content
  - **Auto**: similar to scroll, but adds scrollbars only when necessary
- **Cursor**: Change the shape of the cursor when hovering a mouse over a selected element.
- **Fill**: Change the fill color of a selected element
- **Stroke**: Change the attributes of borders of a selected element


