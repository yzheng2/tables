tables
======
create table market(marketIndex char(50), VariationRange real, OverallCapital real);
//marketIndex represent the index determines trend of market price;
//VariationRange represent the range of change in price of whole market;
//OverallCapital represent the whole capital a market hold in side;

create table stock(Price/share real, OverallShares integer, Variation_Range real);
//Price/share represent stock value per share;
//OverallCapital represent total number of shares the company has;
//Variation_Range represent range of change in price of the stock;

create table company(Cid char(50), MarketValuation real);
//Cid represent unique identify code of a company;
//MarketValuation represent the value of a company in the market;

create table investors(userID char(50), password char(50), Assets real, AmountofShares integer);
//userID represent unique identify code of a investor;
//password is the login permission code;
//Assets represent total amount of money of the investor's account;
//AmountofShares represent total amount of shares in the investor's account;

create table order(userID char(50), Cid char(50), shares integer);
//userID represent unique identify code of a investor make this order;
//Cid represent unique identify code of a company whose stock in this order;
//shares represent the amount of shares transacted in this order;

create table transactionLog(TID char(50), userID char(50), Cid char(50), time date, price real);
//TID represent the unique code of a transaction;
//userID represent unique identify code of a investor make this transaction;
//Cid represent unique identify code of a company whose stock in this transaction;
//time represent when transaction is made;
//price represent how much money is transacted in this transaction;
