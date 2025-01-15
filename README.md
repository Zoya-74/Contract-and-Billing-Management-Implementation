# Contract-and-Billing-Management-Implementation
Developed a system implementation to manage customer contracts and monthly bills, handling term, month-to-month, and prepaid plans with features like deposits, free minutes, and prepaid balances.

# Introduction
MewbileTech Inc. is a new phone company that wants to get a foothold on the Toronto mobile phone market. They are asking for your help in building software to keep track of their historic customer data. They want the program to read in a dataset of customer calls, set geographically in Toronto, and produce a visualization of this past calling activity on a real map of the city. The MewbileTech operator should then be able to filter results, (for example, displaying only calls and texts from a particular customer), or display a detailed bill that a given customer would have been sent during a specific month. We use the term "to filter" to indicate that we want to display only those calls which match the search criterion.

Please note that this is not a "real-time" system where calls would be recorded as they are made but rather a system to visualize calls that have already been made. It is intended for use by a MewbileTech operator to analyze customers' calling patterns.

The classes you will implement include some methods that are never used in the present application, such as a method for cancelling a contract. These provide services that MewbileTech anticipates will be used in future applications.

# Phone Company Specifications
A MewbileTech customer has a unique id number and one or more phone lines. Each phone line has a unique phone number associated with it (which cannot change once assigned to this phone line), a contract, the call history associated with this phone line, and the monthly bill for every month when the line was in use under the current contract. A phone line can change contracts over time, but the application you are writing does not offer that operation to the MewbileTech operator.

A call has a source number, destination number, the time when the call was made, the duration of the call, and the geographic locations (as a pair of longitude+latitude coordinates) of both the source of the call and the destination of the call.

The call history of each customer is a record of all outgoing and incoming calls.

A contract is an agreement between MewbileTech and a given customer. Contracts come in three types: Month-to-Month, Term, and Prepaid. The type of contract determines things like whether the customer must commit to a term (i.e., a period of time), the rate charged per minute of voice time, and the number of included (free) minutes per month. Details on each contract type are provided in Task 3.

A customer can have each of their phone lines under a different type of contract, but each line is associated with exactly one contract.

MewbileTech must be able to bill its customers correctly. A monthly bill has a number of billed minutes, as well as the free minutes included in the customer's contract (if any) that have been used in that monthly billing cycle.

As you will see, the application can display the bill for any customer in any month, it does not have any capabilities related to payments. Each bill is generated assuming there was no unpaid carry-over from the previous month.
