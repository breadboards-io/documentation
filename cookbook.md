# Breadboard Cookbook

## Creating Elements
Breadboard apps are built using Elements and Components. Elements are the basic building blocks of your UI (like boxes, text, or inputs), while Components are more advanced pieces that come with their own pre-set look and logic (like a navigation bar or a custom card).

To add these to your project, you select the element you want from the Dock at the bottom of the screen. Once selected, simply click anywhere on the canvas to place it.
Nesting happens automatically: if you click on an existing element on your canvas, the new one will be placed inside it. This creates a parent-child relationship, allowing you to build complex layouts by layering elements within one another.

<img src="https://cdn.breadboards.app/assets/documentation/cookbook_2.png">

## Responding to Events
You make your app interactive using **Triggers**. A trigger waits for a specific user action, like a click, a hover, or a keystroke, and then runs your instructions.

### Example: A Simple Alert
```
trigger: on click
  Hide me
```

<img src="https://cdn.breadboards.app/assets/documentation/cookbook_3.png">

## Adding Styles and Attributes
You can change how elements look and behave using the **Style Editor** or through **Logic Instructions**.
- **Attributes** ( These are settings or states, like @disabled on a button, a `@placeholder` in a text field, or the `@src` of an image.
- **Styles** ( These are visual properties, like `*background-color`, `*font-size`, or `*opacity`.

In your logic, you can update these instantly to make your UI react to the user:

```
Add @disabled to me
Change Hero Background Color to "blue"
```
<img src="https://cdn.breadboards.app/assets/documentation/cookbook_1.png">

## Displaying Data
To show information to the user, you use the **Change** instruction. Breadboard allows you to "inject" variables or the results of calculations directly into your UI.
If you have a variable called `user_name`, you can display it like this:
```Change Hello Text to user_name```

You can also combine text and variables using the it keyword (which represents the "Result" of the previous step):
```
Combine Text in “Hello” and user_name with the value “ ”
Change my Text to Combined Text
```
<img src="https://cdn.breadboards.app/assets/documentation/cookbook_5.png">

## Conditional Logic
In Breadboard, you don't need complex code for decisions. You use the If instruction to create rules for your app.
```
If my checked is true
  Show #success_message
Else
  Hide #success_message
```

You can also use `Else If` to check multiple rules in a row, or use `AND`/`OR` to combine rules (e.g., `If my checked is true AND user_name is not empty`).
<img src="https://cdn.breadboards.app/assets/documentation/cookbook_4.png">

## Rendering Lists
To display a list of items (like a shopping list or a gallery), you use the `Repeat for each` instruction.
If you have a list of `products`:
```
Repeat for each item in products
  Make a product-card named product_card
  Change Result of make name to product
  Append Result of make name to me
```
<img src="https://cdn.breadboards.app/assets/documentation/cookbook_6.png">

## Updating the Screen (State)
Often, you’ll want your app to "remember" information, like a counter or a user's preference. To do this, you `Create a Variable`.

**Example: A Counter Button**
```
Trigger: On Start
  Create Variable :count with the value 0
  Trigger: On Click
  Increment :count by 1
  Change Count Text to :count
```

Every time you click, Breadboard updates the variable and instantly changes the text on the screen.
<img src="https://cdn.breadboards.app/assets/documentation/cookbook_7.png">

## Sharing Data Across a Screen
Sometimes, different parts of your app need to remember and share the exact same piece of information. In Breadboard, you make a variable **Global** to the current screen by adding a `$` sign to the front of its name.

When you use the `$` prefix, every element on that screen can read from or update that same variable.

**Example: Two buttons, one shared counter**
If you want two separate buttons on a screen to update the same number, use a shared variable like `$count`:
1. On the first button's trigger:
```
Increment $count by 1
Change count_label Text to $count
```
2. On the second button's trigger:
``` Increment $count by 1
Change count_label Text to $count
```



Because you used the `$` sign, both buttons are talking to the same shared memory. If you didn't use the `$`, each button would have its own private counter that the other couldn't see. Using screen-wide variables is the easiest way to keep your UI in sync, such as updating a total price when different items are added to a list.
