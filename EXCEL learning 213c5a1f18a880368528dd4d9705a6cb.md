# EXCEL learning

---

## Date and Time

Data analysts ask date and time-based questions about their datasets, and they can calculate answers using Excel's date and time functions and formulas.

Date and time-based calculations are useful tools in helping businesses to plan for increased demands for products and demands on resources such as staff and equipment. They also help businesses plan towards key dates or deadlines.

 By monitoring daily results over a specific time interval, businesses can identify dips and peaks in performance. For example, a management team might notice that during one period there was a significant drop in sales. If the results are organized by date, they can identify the factors, internal or external, that might have caused this. 

In Excel, each date entry is formatted to appear as a calendar item. However, behind each date is a number that Excel uses to keep track of calendar days. This number is known as a serial number.

![image.png](image.png)

***serial numbers are assigned starting from the 1st January, 1900.***

Excel uses these serial numbers in calculations. Using serial numbers, one date can be subtracted from another to calculate a specific number of days.

**=TODAY()**      makes a dynamic date display in spreadsheet that updates every 24h to display the current **date only.**

**=NOW()**         makes a dynamic date time display in spreadsheet that updates every 24h to display the current **date and time stamp only.**

to extract the date, month and year component of a given date:

**eg. d= 5/8/23**

**=MONTH(A1)**      : 5

**=DAY(A1)**              : 8

**=YEAR(A1)**            : 2023

the Date function/ do not confuse with the above ones; It is used to combine separate date month and year values, when they are given to us separately into a dtetime value.

| month | day | year |
| --- | --- | --- |
| 8 | 31 | 2023 |

**=DATE(C2,B2,A2)    :  08/11/23**

*Lets get started…*

**To actually confirm if a date time value is date time data type:**

1. go to number format box on home ribbon
2. confirm if it is DATE.

**To convert Date time value into serial numbers:**

![image.png](image%201.png)

make it general format from home ribbon.

![image.png](image%202.png)

**DATE difference**

![image.png](image%203.png)

<aside>
💡

Since it is subtraction, the **start date is not included** by default.

</aside>

**CURRENT calc**

have a current date time value, that would be used for as reference.

![image.png](image%204.png)

<aside>
💡

put **‘$’ before row and col. value so that it remains static** or constant when you copy calculations.

</aside>

**Extract year element**

![image.png](image%205.png)

<aside>
💡

use the **autofill** shortcut, 

go to the bottom right, until  the cursor turns into black cross

keep it there and double click 

it does and fill it for al values.

</aside>

**NETWORK DAYS**

if you need to know the number of days available to work on a project, then it’s useful to be able to calculate a result in **working days** rather than calendar days.

NETWORKDAYS uses the country settings on your PC to determine which days constitute a weekend (sat,sun).

Neither **NETWORKDAYS** nor **NETWORKDAYS.INTL** allows for statutory public holidays as there is no information on these days built into the functions. Instead, when creating a formula using these functions, you must include a table of public holidays and reference it in the formula.

***=NETWORKDAYS(start_date, end_date, [holidays])***

![image.png](image%206.png)

**DATEDIF**

The **DATEDIF** function calculates the number of days, months or years between two dates. It is an older function referred to as a “legacy” function in Excel.

## **WORKSHEET**

[[https://docs.google.com/spreadsheets/d/1HUgfgEdsc3GVGL69vnzMagvLnsk17ainwE10Si8yARY/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1HUgfgEdsc3GVGL69vnzMagvLnsk17ainwE10Si8yARY/edit?usp=sharing)](https://docs.google.com/spreadsheets/d/1HUgfgEdsc3GVGL69vnzMagvLnsk17ainwE10Si8yARY/preview?usp=sharing)

---

# LOGICAL FUNCTIONS