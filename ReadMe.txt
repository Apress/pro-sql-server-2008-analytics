The sample database (CONTOSO_MSCRM) needs to be updated and configured. Please read and follow these instructions to allow your account to browse all available data and have queries return results.

1. Read and follow the instructions in the document "Importing the KPITarget Table" in the KPITarget folder, which provides required sample target trends. This issue occurs specifically in exercise 5.1.  
	a. This folder will also contain the "KPITarget" Excel file that needs to be imported.

2. Run this SQL statement against the DB once it’s restored in whatever environment the reader is using:
	
	--Updates a user in the SystemUser table that has full administrative rights
	--Set the DomainName field to your domain/computername and username
	UPDATE SystemUser
	SET DomainName = SYSTEM_USER
	WHERE SystemUserId = '3B0574CE-A5EE-DD11-BDF0-0003FFEB167C'

3. There are multiple instances throughout this book that directs you to "Select 'use a specific user name and password'. 
	a. Set the user name to 'administrator' and the password to 'pass@word1'”. (Refer to page 83 Step 5 as an example). 
	b. After running the UPDATE SQL statement above that gives you administrative rights, enter your credentials (domain or computer name\user and password) instead of the 'admininstrator'.
