
ATM Machine System 

Actors Involved:
1.	Customer:
o	Interacts with the ATM Machine to perform transactions such as withdrawing cash, transferring funds, checking balance, and depositing money.
2.	Technician:
o	Maintains the ATM by refilling cash and performing routine checks to ensure the machine is operating efficiently.
o	Monitors ATM health, ensuring that the machine is functioning properly.
3.	Bank System:
o	Handles transaction authorization through fraud detection and updates balances after successful transactions.
4.	Bank Admin:
o	Monitors and audits transactions for any discrepancies or fraud.
o	Generates reports about the machine's performance and transaction history.
Main Use Cases:
1.	Authenticate User:
o	The system authenticates the user by checking the entered PIN. This is a core function that allows access to further services.
o	Extend/Include:
	If authentication fails, the system will trigger a Handle Authentication Failure use case.
	If successful, the user gains access to various options like withdrawal, transfer, or balance check.
2.	Cash Withdrawal:
o	The customer can withdraw cash after entering the appropriate amount. This transaction is dependent on the ATM having enough cash and the bank system authorizing it.
o	Includes checks for sufficient funds and any fraud detection measures.
3.	Transfer Funds:
o	The customer can transfer funds between their accounts or to other accounts, subject to authentication and fraud detection.
o	Includes:
	Handle Transaction Failure if the transaction cannot be completed (due to insufficient funds or system errors).
4.	Check Balance:
o	The customer can check their balance. This process requires the bank system to retrieve and display the latest balance information.
5.	Deposit:
o	The system allows the customer to deposit money. This function requires physical interaction with the ATM (e.g., inserting cash or checks).
o	Include:
	Print Receipt to give the customer a record of the transaction.
6.	Print Receipt:
o	After transactions, the ATM system can print a receipt as a confirmation and record for the customer.
Supporting Use Cases:
1.	Authorize Transaction:
o	The Bank System is responsible for authorizing the transaction once the customer has initiated it. It checks available funds and prevents fraudulent activities.
o	Includes Fraud Detection to ensure security in every transaction.
2.	Update Balance:
o	Once a transaction is authorized, the Bank System updates the user’s balance to reflect the transaction.
Technician Responsibilities
1.	Refill Cash:
o	Technicians are responsible for refilling the ATM machine with cash when it runs low.
2.	Maintain ATM Machine:
o	Technicians ensure that the ATM is in working order, fixing any mechanical or software issues.
3.	Monitor ATM Health:
o	They monitor the ATM’s health status, addressing any errors or warnings raised by the system.
4.	Perform Routine Checks:
o	Regular maintenance and checks to ensure the machine operates correctly, reducing downtime
Bank Admin Responsibilities:
1.	Generate Reports:
o	The Bank Admin can generate detailed reports on ATM usage, transactions, and performance metrics.
2.	Monitor Transactions:
o	They monitor ATM transactions for suspicious or unusual activity.
3.	Audit Transactions:
o	Bank admins have the responsibility to audit and review transactions, especially for detecting fraud or resolving discrepancies.
System Flow:
1.	Customer Interaction: The customer first enters their PIN, authenticates their identity, and then selects an action (withdrawal, transfer, balance check, or deposit).
2.	Transaction Handling:
o	For withdrawal and transfer, the system processes the requested action, communicates with the bank system for authorization, and either completes the transaction or handles failures (such as insufficient funds).
o	A receipt is printed, and balance is updated.
3.	Technician Monitoring:
o	The technician ensures the ATM is operational and restocks cash or resolves issues as necessary. They monitor the machine health for any errors or failures.
4.	Bank Admin Oversight:
o	The bank admin monitors all transactions, ensuring the machine is secure and that all processes follow established procedures. Reports and audits are used to track and address any discrepancies or potential fraud.
Conclusion:
The ATM Machine system is designed to automate and secure financial transactions while providing ease of access for customers. By involving various actors (customer, technician, bank system, bank admin), it ensures efficient functioning of the ATM, secure transaction processing, and regular maintenance to avoid failures. The system balances security, user convenience, and operational efficiency, making it a crucial part of modern banking services.

