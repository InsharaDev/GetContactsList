# Contact List Lightning Web Component

This repository contains a Lightning web component that retrieves contact records using @wire in an Apex controller and displays them in a lightning-datatable.

## Getting Started

To use this Lightning web component, follow the steps below:

### Prerequisites

- Salesforce Developer Edition or Sandbox org.
- Salesforce CLI installed.
- Access to deploy Apex classes and Lightning web components in your org.

### Setting up Visual Studio Code
 1. Install Visual Studio Code (VSCode) if you haven't already:
 Download and install VSCode from the official website: [https://code.visualstudio.com/](https://code.visualstudio.com/)
 2. Install the Salesforce Extension Pack:
 In VSCode, go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window. Search for "Salesforce Extension Pack" and click Install.

### Installation

1. Clone the repository to your local machine or download the source code as a ZIP file.

2. Authenticate with your Salesforce org using the Salesforce CLI:

  **sfdx force:auth:web:login**

3. Navigate to the root directory of the cloned/downloaded project.

4. Deploy the Apex controller class to your org using the following command in VScode:
     
  **sfdx force:source:deploy -u [username] -p force-app/main/default/classes/ContactController.cls**

5. Deploy the Lightning web component to your org using the following command in VSCode:

  **sfdx force:source:deploy -u [username] -p force-app/main/default/lwc/contactList**

6. Open your Salesforce org.

7. Create a Lightning page or open an existing Lightning page where you want to add the Contact List component.

8. Add the Contact List component to the Lightning page:
- Click on the "Edit Page" option.
- Drag and drop the "Contact List" component onto the desired section of the page.
- Save and activate the Lightning page.

9. Navigate to the page where you added the Contact List component and verify if the contact records are displayed correctly in the lightning-datatable component.

## Usage

The Contact List Lightning web component retrieves contact records from the Salesforce org and displays them in a table. The component automatically fetches the contact records when the page loads.

To refresh the data, you can click on a "Refresh" button or invoke the `refreshData()` method in the JavaScript controller.

## Component Customization

If you need to modify the fields displayed in the lightning-datatable, you can update the `columns` array in the `contactList.js` file.


  
