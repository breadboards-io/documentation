# Breadboard Cookbook

## Creating Elements
Breadboard apps are built using Elements and Components. Elements are the basic building blocks of your UI (like boxes, text, or inputs), while Components are more advanced pieces that come with their own pre-set look and logic (like a navigation bar or a custom card).

To add these to your project, you select the element you want from the Dock at the bottom of the screen. Once selected, simply click anywhere on the canvas to place it.
Nesting happens automatically: if you click on an existing element on your canvas, the new one will be placed inside it. This creates a parent-child relationship, allowing you to build complex layouts by layering elements within one another.

## Responding to Events
You make your app interactive using **Triggers**. A trigger waits for a specific user action, like a click, a hover, or a keystroke, and then runs your instructions.

### Example: A Simple Alert
```
trigger: on click
```
