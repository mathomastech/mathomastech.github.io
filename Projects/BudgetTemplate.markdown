---
layout: project
title:  "Budget Template - Google Spreadsheet"
category: "project"
author: "Marc Thomas"
date:   2013-07-27 12:00:00
categories: Budget Financial Finances Spreadsheet Google Drive Docs
---
<p class = "projectHeader">
In the following links, you will find details for each type of page in the template. The 2 most complicated are "Projections", and "Loan Projections". The "Overview" sheet also has some unique behavior. The remaining sheets are similiar enough that learning one will help you use the others.
</p>
<p></p>
<ul class = "projectQuickLinks">
    <li><a class="projectPage"  href="https://docs.google.com/spreadsheet/ccc?key=0AnHTaegW0AL-dE15NHhHUkhyREUwSENTWHZqQmFFTlE&amp;usp=sharing">Link to project</a></li>

    <li><a class="projectPage"  href="#Overview">Overview</a></li>

    <li><a class="projectPage"  href="#Projections">Projections</a></li>

    <li><a class="projectPage"  href="#LoanProjections">Loan Projections</a></li>

	<li><a class="projectPage"  href="#IncomeExpenses">Income</a></li>

	<li><a class="projectPage"  href="#Expenses(B)">Expenses (Type B)</a></li>
</ul>

<a id="Overview"></a>
##Overview##

<a href="/img/BudgetTemplate/BudgetOverview.png" data-lightbox="BudgetOverview"><img src="/img/BudgetTemplate/BudgetOverview.png" alt="Budget Overview" width="800" height="300"/></a>

<p class="projectContent">
The overview is your landing page, and also one of the most useful. While you don't edit much here, this is where you can begin to understand how your money is being spent. There are a few things you need to do here for setup and maintanence and they are:</p>
<p></p>
<ol class="projectContent">
	<li><strong>Set your year.</strong></li>
		<ul>This is critical as there are several other sheets that rely on the year you enter. Namely <strong><em>Projections</em></strong> and <strong><em>Loan Projections</em></strong>. Simply enter "2013" or whatever year you are using this budget for.</ul>
	<li><strong>Add your starting balance.</strong></li> 
		<ul>This number is added to your total balance, but is not included in any specific month's income. This way it won't skew data.</ul>
	<li><strong>Add your balances next to the "Bank 1" and "Bank 2" cells.</strong></li>
		<ul>If you have more than two balances (i.e. Personal Saving account and Personal Checking account, Spouses Checking Account, etc,) then you can add more cells as needed. Just don't forget to modify the <strong><em>Total:</em></strong> formula accordingly.</ul>
</ol>
<p></p>
<p class="projectContent">
The remainder of this sheet is completely automated. After initial setup, this is how best to use the sheet. Whenever you make purchases, be sure to update the balances of your respective accounts. The budget will then compare your balances with how much income/expenses you have logged throughout the budget. If everything was logged correctly, the variance will be <strong><em>$0.00</em></strong>. If there are mistakes in any logged items, there will be a variance, and you will have to go through and find it.

Off to the right, you will see <strong><em>Avg/Month</em></strong>. Use this to estimate how much you spend or make in a certain category per month. Next is <strong><em>Maximum</em></strong>. While I have not found a legitamate use for this yet, I do find it and interesting data point. Lastly, <strong><em>Percentage</em></strong>. This one is very useful, as it will tell you how much money you spend in each category in relation to every other category. It does the same for income, so you can guage just how much of your money comes from or goes to a particular piece of your budget. Using this, I have noticed that I spend a significant percentage more than I realized on restuarants. Since realizing that, I have been working to decrease that and have had some success.
</p>

<a id="Projections"></a>
##Projections##
<a href="/img/BudgetTemplate/Projections.png" data-lightbox="Projections"><img src="/img/BudgetTemplate/Projections.png" alt="Projections" width="800" height="300"/></a>

<p class="projectContent">
The projections page is something I began work on a few months ago as a tool to help me predict/anticipate my finances in the coming months, and coming years. To begin, first you need some starting informaion, namely what are your recurring expenses. If you look to the far right of the sheet, you will find four columns for recurring expenses. </p>
<p></p>

<ol class="projectContent">
	<li><strong>Recurring Expenses:</strong></li>
		<ul>This is your category field. There are a handful of default items, but you can change these or add more as you see fit. *Note: Changing these default categories will cause the "Projected Remaining" column to give you false information.</ul>
	<li><strong>Projected Recurring:</strong></li>
		<ul>This is an estimate of how much money you spend on each category. It will apply the sum of all these costs as your recurring expenses for all future months (not including the current month)</ul>
	<li><strong>Projected Current:</strong></li>
		<ul>This is an estimate of how much you are budgeting for each category for the current month. Use this to adjust your values throughout the month to make your budget. If you know you will be short on income, it is a great way to find ways of saving some money by cutting extra expenses.</ul>
	<li><strong>Projected Remaining:</strong></li>
		<ul>This column tells you how much money in each category remains to be spent for the current month. The calculation takes the value from <strong><em>Projected Current</em></strong>, subtracts to current months total expenses in the category based on the value from the overview page, and returns the different. It will zero out if you have no remaining funds in that category.</ul>
</ol>
<p></p>
<p class="projectContent">
	*Note: As stated earlier, if you change the category names, the formula to compare the Projected Current and the overview values will not be comparing correctly. You will need to adjust the formula to substract from the correct row.
</p>
<p></p>

<a id="LoanProjections"></a>
##Loan Projections##
<a href="/img/BudgetTemplate/LoanProjections.png" data-lightbox="Loan Projections"><img src="/img/BudgetTemplate/LoanProjections.png" alt="Loan Projections" width="800" height="300"/></a>

<p class="projectContent">
	The loan projections page is something new I've been working on to help predict how long it will take to pay off loans, credits cards, or other forms of outstanding balance payments. To use this, start by renaming <strong><em>Loan 1</em></strong> to the name of your loan, for example "Chase Card". Put your current outstanding balance in the <strong><em>Current Balance</em></strong> column. Add in your Annual Percentage Rate (APR), and your monthly expected payment.  The title of the Loan will automatically change in the first row. From there, the current balance minus the months payment will be inserted into the current months cell. All following cells will populate with the balance of the previous month minus the payment plus interest. If you want to make an alternate payment for a specific month, either more or less than your default, you can put that number in the "Alt Payment" column and it will automatically adjust the current month, and all following months accordingly. Whenever a loan is completely payed off, it will zero out the balance of that loan for all future months. This is a great way to figure out how long it will take to pay off outstanding balances at any given recurring payment value, and how much additional payments of a specific value will effect the balance of the loan months or years in advance. By default, 4 loans are displayed, however you can have as many as 10 by unhiding the columns. 
</p>

<a id="IncomeExpenses"></a>
##Income and Expenses (Type A)##

<a href="/img/BudgetTemplate/Income.png" data-lightbox="Income"><img src="/img/BudgetTemplate/Income.png" alt="Income" width="400" height="300"/></a>

<a href="/img/BudgetTemplate/Expenses1.png" data-lightbox="Expenses1"><img src="/img/BudgetTemplate/Expenses1.png" alt="Expenses1" width="400" height="300"/></a>

<p class="projectContent">
	The <strong><em>Income and Expense (Type A)</em></strong> are nearly Identical. To use, simply put you income/expenses in the row with the appropriate month name, the date of the log entry (Not required, but I have found it useful) and add a description of the log (also not required, but useful). The overview will automatically populate based on the values logged in these pages.
</p>

<a id="Expenses(B)"></a>
##Expenses (Type B)##
<a href="/img/BudgetTemplate/Expenses2.png" data-lightbox="Expenses2"><img src="/img/BudgetTemplate/Expenses2.png" alt="Expenses2" width="800" height="300"/></a>
<p class="projectContent">
	Nearly identical concept to <strong><em>Income and Expense (Type A)</em></strong>, the only different is the layout. Sheets that use this layout are for categories that only have 1 payment each month. Unlike something like restaurants where you may log in 10 or 20 restaurant expenses, you will only be paying a phone or electric bill once per month. Totals are agregated so you can see how much you are spending each month for all items in this category (row total), as well as how much you have spent all year for a specific item in the category (column total).
</p>
