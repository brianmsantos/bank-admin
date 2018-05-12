BANK ADMIN
You're starting a bank and you need a way to manage your clients and all the deposits and withdrawals that are going to happen. Since you're in a web development course, let's use software!

Data/API Requirements
You will use sequelize to model and support create and read operations for three types of records: user, account, transaction.
A user record should store the person's name and address. A user may have multiple accounts.
An account record should have a name and type (ex. 'checking', 'savings') and belongs to one user.
A transaction is associated with one account, can represent a deposit or withdrawal, and should have a description.
UI Requirements
Your index/homepage (ex. localhost:8080/) will show a list of all users along with the accounts they own and the type, name, and current balance for each account.
You will need a page (ex. /create_transaction) that lets you create a transaction to enter a deposit/withdrawal for a particular account.
You will want a page where you can view the balance and all transactions for a single account (ex. /accounts/3/summary)
Bonus ideas: support transfers between accounts, implement account minimums with an automatic overdraft fee, add support for searching transactions
Directory Setup Tips
Make a new directory for your project and cd into it.
Initialize your sequelize directories (and auto-create the index.js model loading script) by running sequelize init:models & sequelize init:config. If this produces an error, then you may not have the sequelize and the sequelize-cli installed globally. Fix this by running npm install -g sequelize sequelize-cli in your terminal and trying again.
Create a package.json by running npm init -y
Create a .gitignore file
Database Setup Tips
Make a schema.sql which creates a new database and run it, or create the new database manually in SQL Workbench or the command line (mysql).
You will probably to seed your tables with some initial data to test your API and UI. You can do this by making a seed.sql script and running it, or manually enter some records.
The rest ... Up to you!
Look at our sequelize activities and other past activities for ideas and help
You need to support user, account, and transaction records but the actual model/schema is up to you.
For the UI, want to use Handlebars to render HTML server-side? Or serve static HTML and use ajax calls to fetch data and render your UI client-side? Maybe a mix of both? Go for it.
Talk to your neighbors, Google for answers, check Stackoverfow, read the docs (Sequelize, Express, Handlebars)
Want to review a particular topic or get help with an error/issue? Call an instructor/TA over.