# MAST-assignment-part-2
1.	Scenario Analysis
Requirement	Your Response
Who will use the application?	The application will be used by the chef at Christoffel's local restaurant.
What is the purpose of the application?	To replace the current paper-based system and make menu management easier by allowing the chef to update dishes, organise the menu, and quickly find information.
What information must the application store?	It must store details for each menu item, specifically the Dish Name, Description, and Course (Starter, Main Course or Dessert), as well as the Price.
List four functions the application should perform.	1. Add new menu items.


2. View all menu items.


3. Edit menu items.


4. Delete menu items.

List two usability requirements the application should have.	1. The application must provide helpful validation and feedback messages.


2. The application must provide an improved user experience.


1.	User Interface Design
Screen 1: The Menu Dashboard
This will be the main screen the chef sees when opening the app, used for viewing and managing the list of dishes.
•	Screen Title: "Menu Manager" or "Current Menu".
•	Text Field: A search bar at the top to quickly find specific dishes.
•	Dropdown/Picker: A filter option below the search bar to sort the view by Course (Starter, Main, Dessert).
•	List: The main body of the screen displaying the current menu items. Each item in the list should display the Dish Name, Course, and Price.
•	Button: A clearly visible "Add New Item" button (a floating action button at the bottom right usually works great for mobile layouts).

 
Screen 2: Add / Edit Dish Form
This screen handles data entry and validation when the chef is adding a new recipe or updating an existing one.
•	Screen Title: "Add New Dish" (or "Edit Dish" when updating).
•	Labels & Text Fields:
o	"Dish Name" label paired with a standard text input.
o	"Description" label paired with a multiline text input.
o	"Price" label paired with a numeric text input.
•	Dropdown/Picker: A "Course Type" picker allowing the chef to select Starter, Main Course, or Dessert.
•	Labels (Validation): A dedicated text area (perhaps in red text) near the save button for displaying helpful feedback or error messages if the chef misses a required field.
•	Buttons: A primary "Save Dish" button and a secondary "Cancel" button to return to the dashboard.
 
2.	Application Flow
 
3.	React Native Component Planning
Application Requirement	React Native Component	Purpose
Display a head
ing	<Text>	Renders styled text on the screen to display section titles and headers like "Current Menu" or "Add New Dish".
Enter the dish name	<TextInput>	Provides a single-line text input field for the chef to type the name of the dish.
Enter the description	<TextInput multiline="{true}">	Provides a multi-line text field allowing the chef to type out longer detailed descriptions for each dish.
Select a course	<Picker> (from @react-native-picker/picker)	Renders a dropdown menu allowing the user to choose a course option (Starter, Main Course, or Dessert).
Enter the price	<TextInput keyboardType="decimal-pad">	Captures numerical input for dish pricing using a dedicated numeric keyboard layout.
Save a menu item	<TouchableOpacity> (or <Button>)	Creates an interactive button that triggers the save handler function to validate inputs and update the menu array state.
Display menu items	<FlatList>	Renders a dynamic, scrollable, and memory-efficient list of all stored menu items.

4.	The Code of the app.
For the first screen.
 
 
 
 
 
 
 
 

Second screen code.

 
 
 
 
 
 
 
 
 



6. Design Reflection

Design Reflection
The proposed application design directly addresses Christoffel’s restaurant operational challenges by replacing an inefficient paper-based menu with a streamlined, digital management tool. Designed specifically for fast-paced kitchen environments, the app allows the chef to easily view, add, edit, filter, and delete dishes in real-time. Built-in search and course filtering further reduce cognitive load during hectic service hours. By structuring the core user flow around simple management tasks, the layout ensures instant access to critical dish details—including dish names, descriptions, course categories, and prices—eliminating paper clutter and improving operational organization.
The deliberate choice of React Native components plays a fundamental role in maximizing overall usability and interface clarity. Using a <FlatList> component delivers a smooth, performant scrolling experience for dynamic menu data, keeping memory usage minimal as the restaurant’s catalog grows. For data entry, tailored <TextInput> components (utilizing keyboardType="decimal-pad" for price inputs and multiline formatting for descriptions) streamline data entry while minimizing input errors. The <Picker> component standardizes course selection into a straightforward dropdown, eliminating spelling inconsistencies and guaranteeing accurate menu categorization. Furthermore, <TouchableOpacity> elements provide immediate visual touch feedback, giving the chef tactile confidence when saving updates, canceling actions, or removing dishes. Finally, clear <Text> labels deliver immediate error validation messages, producing an intuitive, user-friendly mobile application tailored for daily kitchen use. This thoughtful integration guarantees a cohesive system that scales gracefully with future restaurant requirements.


Youtube link. 
https://youtu.be/P1nxRPYRDXc

GitHub repo link. 
https://github.com/ST10494404/MAST-assignment-part-2.git



Reference List
Boduch, A. and Derks, R. (2020) React and React Native: Harness the power of React Native to build attractive and scalable hybrid applications. 3rd edn. Birmingham: Packt Publishing.
Cooper, A., Reimann, R., Cronin, D. and Noessel, C. (2014) About Face: The Essentials of Interaction Design. 4th edn. Indianapolis, IN: John Wiley & Sons.
Kasavana, M.L. (2016) Managing Technology in the Hospitality Industry. 7th edn. Lansing, MI: American Hotel & Lodging Educational Institute.
Meta Open Source (2024) React Native Documentation: Core Components and APIs. Available at: https://reactnative.dev/docs/components-and-apis (Accessed: 8 September 2026).
Nielsen, J. and Budiu, R. (2013) Mobile Usability. Berkeley, CA: New Riders.
Norman, D.A. (2013) The Design of Everyday Things. Revised and expanded edn. New York: Basic Books.
Pressman, R.S. and Maxim, B.R. (2020) Software Engineering: A Practitioner's Approach. 9th edn. New York: McGraw-Hill Education.
React Native Community (2024) @react-native-picker/picker. GitHub repository. Available at: https://github.com/react-native-picker/picker (Accessed: 8 September 2026).
Robertson, S. and Robertson, J. (2012) Mastering the Requirements Process: Getting Requirements Right. 3rd edn. Upper Saddle River, NJ: Addison-Wesley.
Shneiderman, B., Plaisant, C., Cohen, M., Jacobs, S., Elmqvist, N. and Diakopoulos, N. (2016) Designing the User Interface: Strategies for Effective Human-Computer Interaction. 6th edn. Boston: Pearson.
Sommerville, I. (2016) Software Engineering. 10th edn. Boston: Pearson.
Tidwell, J., Brewer, C. and Valencia, A. (2020) Designing Interfaces: Patterns for Effective Interaction Design. 3rd edn. Sebastopol, CA: O'Reilly Media.
onal South African fried dough dish
vetkoek




