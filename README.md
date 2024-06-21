##Overview
This project aims to create a system for managing programs and their associated items in Frappe. Each program can have multiple items, and the system allows for easy addition and updating of these items using custom buttons and dialog boxes. The project involves creating two Doctypes: Program (parent) and Program Item (child), with the Program Item linked to the Program Doctype.

##Features
Parent Doctype: Program
Fields: Program Name, Program Items (linked to Program Item)
Child Doctype: Program Item
Fields: Item Group, Item (filtered by Item Group), Item Name (fetched from Item), Quantity, Finish, Description
Custom Buttons and Dialogs
"Add New Item": Opens a dialog to add new program items.
"Update Item": Opens a dialog to update existing program items.
Installation
Prerequisites
Ensure you have a Frappe environment set up. If not, follow the official Frappe installation guide: Frappe Bench.

1. Clone the Repository
Clone the existing repository containing the custom app:

sh
Copy code
git clone [repository-url]
2. Install the Custom App
Navigate to the bench directory:

cd /path/to/bench
Install the app:

bench get-app program_management /path/to/repo/program_management
bench --site [your-site-name] install-app program_management
