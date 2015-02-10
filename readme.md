#Address book

Create a new app using Sails, Angular, and MongoDB to store addresses.

This should be a "single page app" created using a combination of ngRoute and modals.

##Backend

The backend of this app will be created using sails.js and should only require 1 model called `contact` and 1 view.

##Contact model

Each contact should have the following data:

* First Name
* Last Name
* E-mail
* Street Address
* City
* State
* Zip
* Phone
* Notes


All create/update forms should have fields for all of these attributes and have some sort of validations on the server (model) and frontend (angular).

##Home page

Route: `/`

Displays a list of all of the people in your address book. Should just be a list of peoples basic details (First Name, Last Name, and Company).

The list will also have a view, edit, and delete button.

**Delete** should be done via AJAX and the list should update without a page refresh

**Edit** should be done with a form in a modal and the list should update when they save the item. The modal should have Save and Cancel.

**View** view should link to a new URL (View Contact Page) so you can link directly to people's entry in the address book by id.

##View page

Route: `/contact/:id`

Should display the full details of the entry in the address book. Should have a back button (returns to home page) and an edit button (edits the current item with the same modal used on the home page).
