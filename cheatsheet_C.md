# Cheatsheet for C analysis

## Table of contents

* [Interger overflow](#integer_overflow)

## Integer Overflow <a name="integer_overflow"></a>

Following code is vulnerable to an unsigned interger overflow :

* *total_cost* is defined as a 4 bytes unsigned integer (values between -2,147,483,648 and 2,147,483,647).
* *total_cost* value is controlled by the user (`total_cost = 900*number_of_articles;`).
* if *total_cost* exceed the unsigned int range, a negative value could be returned and added to the user balance (For example : if the user buy 2,386,095 articles).

```C
int account_balance = 1100;
int total_cost = 0;
int number_of_articles = 0;

fflush(stdin);
scanf("%d", &number_of_articles);

total_cost = 900*number_of_articles;
printf("\nThe final cost is: %d\n", total_cost);

if(total_cost <= account_balance){
    account_balance = account_balance - total_cost;
    printf("\nYour current balance after transaction: %d\n\n", account_balance);
}
```
