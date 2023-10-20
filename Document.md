# UserInterfaceDocument
This document outlines the requirements and specifications for the User Management screen of this application.

-> Requirements
When we look at the interface, we can see that administrators generally create an interface based on creating users and listing users. But the interface has some needs:
1. First of all, users' details can be entered, but some information (phone number, etc.) cannot be displayed during listing.
2. I did not observe any area for editing, deleting user details or deactivating the user.

-> UI Components
1. User List
   The table displaying the list of user accounts. The list has ID, User Name, Email, Enabled columns.
3. User Details
   The separate page for entering details of user accounts. It has "New User", "Username:", "Displayname:","Phone:","Email:","User Roles:","Enabled:" textboxes. It has Fields for each of them that take inputs except "Enabled:" textbox. "Enabled:" textbox has a checkbox. Also There is "Hide Disabled User" checkbox.
5. User Actions
    Finally there are Save User and New User buttons."Enabled:" textbox has a checkbox. Also There is "Hide Disabled User" checkbox. Save User Button sends inputs to User List, New User Button clears all inputs and updates the User List. "Hide Disabled User" checkbox updates User List with hiding user accounts that have the column "false" for Enabled.

-> Page Behaviour
1. When the page loads, it should display the list of user accounts sorted by username in ascending order.
2. Clicking on the "Create User" button should open the User Details modal/page to create a new user.
3. After the information is entered, the table and inputs are updated with the "Save User" button.
4. Sorting the table should reorder the user accounts based on the selected column.(ID)

-> Initial Page View
When the User Management screen first loads, it should display a table of user accounts sorted by username in ascending order. No specific user account details should be displayed initially.
