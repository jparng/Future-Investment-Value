# Future-Investment-Value
       
The problem was to write a script that would prompt the user to add values for the investment amount, annual interest rate,
and the number of years and then calculate the future investment value using this formula: 

futureInvestmentValue = investmentAmount * (1 + monthlyInterestRate)numberOfYears*12 

The user would input the investment amount, annual interest rate, and the number of years when prompted,
and the program would output the future investment value and display the line
“Accumulated value is” with the number that was processed through the formula. 
Since the user was only inputing an annual interest value,  another formula had to be used : 

monthlyInterestRate = (annualInterestRate/ 12) / 100 
[Divide by 12 for each month and then divide by 100 for the percentage value] 


Once monthly interest rate was calculated, the program would be able to calculate the future investment value. 
  
  
 
Design: 
1. Ask the user to input three values that would be saved as variables: 
Investment amount --> investmentAmount 
Annual interest rate --> annualInterestRate 
Number of years --> numberofYears 
  
2. Find the monthly interest rate using the formula: 
monthlyInterestRate = (annualInterestRate/ 12) / 100 

3. Calculate the future investment value through the formulas: 
futureInvestmentValue = investmentAmount * (1 + monthlyInterestRate)numberOfYears*12 

4. Separate into simpler equations with : 
x = (1 + monthlyInterestRate) 
y = numberOfYears * 12 
futureInvestmentValue = investmentAmount * x^y 

5. Displays the result and made sure to keep the value rounded with the line "Accumulated value is " +  Math.round(futureInvestmentValue * 100.0) / 100.0). 
