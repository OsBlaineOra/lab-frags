# Create an ATP instance

You will need a database to complete the exercises.  An Oracle Autonomous Database handles a lot of the background admin tasks for you so you can focus on your project.

1. Click "Create an ATP database" in the Autonomous Transaction Processing box.  
   ![OCI Cloud Dashboard](images/cloudDashboard.png)
1. Choose your new compartment.
1. Enter `MyAtpDb` in Display name
1. Enter  `MyAtpDb` in Database name
1. Make sure "Transaction Processing" is selected.
1. Make sure "Shared Infrastructure" is selected.  
   ![Create ATP form 1](images/createATPForm1.png)
1. Scroll down to "Configure the database" select "Show only Always Free configuration options"  
   ![Create ATP form 2](images/createATPForm2.png)
1. Scroll down to "Create administrator credentials".  Enter and confirm the ADMIN password.  
   **Note:**  the Admin account is the top level user for your new database.  Create a strong password and keep it secure.
1. Scroll to the bottom and click "Create Autonomous Database".  
   ![Create ATP form 3](images/createATPForm3.png)  
   You will receive an email when your new ATP Database instance has been provisioned.
1. Locate your new database's OCID and click Copy.
   ![Copy Database OCID](images/dbOcid.png)  
