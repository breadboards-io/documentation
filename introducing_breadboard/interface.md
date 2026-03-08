# Interface

Breadboard works on web browsers - no need to download an app. This allows effortless UI asset importing and AI support.

### Layer Panel
<img width="6048" height="3928" alt="01_Interface_1" src="https://github.com/user-attachments/assets/3756433d-1969-407d-a417-45ac734b793e" />

The layer panel provides an overview of all the frames and layers created or imported, organized based on their hierarchy. Adding layers can be done in several ways. You have the option to import layers from your design tool, copy UI assets as styled HTML or  SVGs, or add them through the dock UI. 
When importing designs from Figma, Sketch, or any design tool , the layer hierarchy remains intact, preserving the structure from the original design file. 

#### 💡 Pro-Tip

When it comes to the layer selection with the mouse cursor, the topmost layer will be selected first and then double-clicking the layer multiple times to get down to layers underneath. If you want to select the child layer directly, simply ctrl+mouse click the target layer.

### Style editor
<img width="6048" height="3928" alt="01_Interface_2" src="https://github.com/user-attachments/assets/4dcfef46-6e3f-4d40-8900-05ada86e87d7" />

The style editor allows you to create screen interfaces from scratch or to edit imported UI designs from your favorite design tool(s). For more detailed features of the style editor, check ‘Import UI assets’ article.  You can also add and combine properties to components you created. For the detailed information about properties, check ‘Create and combine properties’.

### Canvas
<img width="6048" height="3928" alt="01_Interface_3" src="https://github.com/user-attachments/assets/5bf7f028-d1b4-4b27-9039-44786ceb30dc" />

The canvas is the main space where you display all layers and containers and let you connect logic with each of them. Just like any open-canvas design tools, you can tweak your screen designs and create multiple boards. To navigate within the canvas, you can easily pan around by clicking and dragging on the screen.

At the bottom of the canvas you can find the dock UI that provides the main tool options. Here you can find:

- <img width="32" height="32" alt="01_Interface_4_2" src="https://github.com/user-attachments/assets/4ebbb53c-db19-447a-b1fd-c8527b2a77e4" />  **Design mode**: The default mode for editing UIs and logics
- <img width="32" height="32" alt="01_Interface_4_1" src="https://github.com/user-attachments/assets/f7841515-7464-4f49-ad29-15ebea7b739b" />   **Run mode**: Previewing the app you made. If your app has multiple screens, the app will start from the ‘Entry point’ and flow to other pages by your logic automatically. (Note: Editing UI/logic is not doable in this mode.)  
- <img width="32" height="32" alt="01_Interface_4_3" src="https://github.com/user-attachments/assets/c4ed92c2-fed8-444c-ad2d-d4a00f56805f" />  **Add screen**: Add more screen to the canvas. The first added screen is set as ‘Entry point’ by default, but you can change the entry point after adding a new screen.
- <img width="32" height="32" alt="01_Interface_4_4" src="https://github.com/user-attachments/assets/fcec6624-884d-48f9-9973-04cc452c763a" />  **Add element**: Add UI component presets or custom UI component that you created to the screen. Here you can find:
  - Container: A structural building block that can be fully styled using the style editor and used to group or hold other elements inside it.
  - Text: A normal text box
  - Input: A variety of input forms used to enter data. Interacting with it can trigger system UIs like device keyboard, date picker, etc.
  - Button: An interactive, clickable element
  - Media: A placeholder for images/videos/audios
  - Component: Custom, reusable UI components that you’ve created on canvas
- <img width="32" height="32" alt="01_Interface_4_5" src="https://github.com/user-attachments/assets/0013b62a-0df9-4f4f-9410-aecc0b472711" />  **AI agent**: Toggle Rubber Duck AI agent  

### Logic panel
<img width="6048" height="3928" alt="01_Interface_5" src="https://github.com/user-attachments/assets/23097419-3f3e-489f-a91b-39d9d12348a0" />

The logic panel is the pinnacle of Breadboard - In Breadboard, logic expressions are event-oriented, making the logic as easy to follow as a conversation. To add logic blocks to a UI element/container/body etc., simply click on the target from the canvas and tap “Add Trigger” to add events and then tap “Add Actions” to build logic.  Learn more about logic commands in the ‘Logic editor’ section.
