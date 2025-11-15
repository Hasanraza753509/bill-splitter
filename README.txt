Bill Splitter

This is a single-page web application designed to quickly and easily split a bill among a group of people. It calculates who owes whom and provides the most optimized list of transactions to settle all debts with ease.
This tool is perfect for splitting rent, dinner bills, vacation costs, or any other shared expense.

Features

* Dynamic Payer List: Easily add or remove people from the bill.
* Simple Input: Just enter each person's name and the total amount they paid.
* Clear Summary: Instantly see the Total Bill, Total People, and the Cost Per Person.
* Optimized Settlements: Instead of everyone paying a central person, this tool calculates the fewest possible transactions needed to settle all debts.
* Responsive Design: A clean, dark-mode interface that works on both desktop and mobile.
* Helpful Feedback: Provides clear success and error messages (e.g., "Everyone is settled up!", "Total bill must be greater than ₹0.").
* Localized Currency: All amounts are formatted in Indian Rupees (₹).


How to Use

Since this is a self-contained HTML file, there is no installation or build step required.
1. Download: Save the index.html file to your computer.
2. Open: Open the index.html file in any modern web browser (like Google Chrome, Firefox, or Safari).
3. Add Payers: Use the "Add Person" button to add a row for everyone who paid a portion of the bill.
4. Enter Data: Fill in the name of each person and the amount they paid.
5. Calculate: Click the "Calculate Split" button.
6. View Results: The app will instantly display the summary and a list of transactions showing exactly who needs to pay whom to settle the bill.

🧠 How It Works: The Settlement Logic

The "advanced" part of this splitter is its settlement algorithm, which minimizes the number of payments.
1. Calculate Balances: The app first calculates the total bill and the average cost per person. It then determines each person's balance:$Balance = Amount Paid - Average Cost$
2. Identify Debtors and Creditors:
    * Anyone with a negative balance is a Debtor (they owe money).
    * Anyone with a positive balance is a Creditor (they are owed money).
3. Sort Lists: The app sorts debtors by who owes the most and creditors by who is owed the most.
4. Match Transactions: It uses a greedy algorithm to match the largest debtor with the largest creditor, transferring the minimum of the two amounts. This process repeats until all balances are (close to) zero. This ensures that money moves in the most efficient way possible, resulting in the fewest transactions.
