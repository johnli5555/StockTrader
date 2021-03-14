# StockTrader
1. Creates 3 tables in the database

  1.1 Client table          
        ClientID	FirstName	 LastName	 UserName  Email	Mobile	BirthDate	Password
 	 	 	 	 	 	 	 
  1.2 Client Account Table
        ClientID	AccountNo	Investment  	Cash	Balance	Date	Description
 	 	 	 	 	 	 
  1.3 Stock Portfolio Table
       ClientID	Ticker	PurchasePrice    TradeDate	 CurrentPrice	Change%	Quantity	Total

  I don't have a DB like MySQL or MongoDB in my laptop. So I am using static data.

2. The StockTracking.html is the system starting point. Click it, then the login page will appear. 

  2.1 when you enter Username as "John" and Password as "555888". then click Login, your account info page will display.
     (should query Client table using username, if found, check password. if password match. It lets the user login. otherwise, the system shows an error message)

  2.2 When you enter other than Username as "John" and Password as "555888", you will get error message: "Error Password or Username. Please click OK to register first".
      Click OK, then the resgister page opens.

3. The resgister page

  3.1 User name must be great than 5 characters. Otherwise, an error message is displayed "your userid must great than 5 characters".

  3.2 For security reasons, your password must between 8 to 15 characters an contains at least one lowercase letter, one uppercase letter, one numeric digit, and one special character. 
     If your password does meet the security requirments, you will get the alert message.

  3.3 If your username and password both meet the security requirements, you will get a message "You are successfully registered! Please log in and start to invest". 
     then you are redirected to the Add Money page.

4. Add Money page

  4.1 Enter an amount of money in the "Add balance to your wallet" box. Click the "Submit" button, your amout will show under the current balance in your wallet. (Should add your bank balance)

  4.2 Click button "Check Balance", you can see your investment portfolio. (Query database, displays a portfolio report)

  4.3 Click the button "Google", you will go to Google Finance page. Here, you can search stock live rates. (Call API to Stock Trading System such as TSE, NYSE or NASDAQ 
     to get the live rate of the stock, it will appear onscreen)

5. Buy/sell shares (Not finished yet. Still building a trading page, allowing users to set their order, the calls Stock Trading System API to commit your transaction)
      
 	 	 	 	 	 	 	 
