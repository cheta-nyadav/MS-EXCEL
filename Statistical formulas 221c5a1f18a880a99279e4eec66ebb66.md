# Statistical formulas

![image.png](image.png)

![image.png](image%201.png)

### Q1. Calculate the total no of transactions per each state. (COUNTIF)

so we need to count the number of transactions only, so we need to count the no of occurrences of each state, and use count or to be more specific count if.

step1. Get all distinct state names from there.

1. copy the state col to a new col.
2. use remove dulicates to get distinct states
3. use COUNTIF to sum the state transactions.

![image.png](image%202.png)

![image.png](image%203.png)

![image.png](image%204.png)

![image.png](image%205.png)

### Q2. Calculate total trans. by each state and prod category (COUNTIFS)

so we need 2 level of aggregating, by state and prd category. so we’ll find distinct states and distinct prod category, then we can represent them as either:

| Maharashtra | Furniture |
| --- | --- |
|  | Stationery |
|  | Clothing |
|  | Groceries |
|  | Electronics |
| Tamil Nadu | Furniture |
|  | Stationery |
|  | Clothing |
|  | Groceries |
|  | Electronics |
| Karnataka | Furniture |
|  | Stationery |
|  | Clothing |
|  | Groceries |
|  | Electronics |

|  | **Furniture** | **Stationery** | **Clothing** | **Groceries** | **Electronics** |
| --- | --- | --- | --- | --- | --- |
| **Maharashtra** |  |  |  |  |  |
| **Tamil Nadu** |  |  |  |  |  |
| **Karnataka** |  |  |  |  |  |
| **Gujarat** |  |  |  |  |  |
| **Delhi** |  |  |  |  |  |

sow have two condition, one on state and one on prod category, so we use COUNTIFS instead,

=countifs($D:$D,$O17,$F:$F,P$16)

<aside>
💡

for expanding along a row, we need to fix $ col,and vice versa

</aside>

![image.png](image%206.png)

![image.png](image%207.png)

### Q3. Calculate the total quantity sold by regions. (SUMIF)

find distinct regions, and apply sum if on quantity column.

![image.png](image%208.png)

### Q4. Calculate the total quantity sold by region and product name. (SUMIFS)

=SUMIF(sum range, criteria range 1, criteria 1, criteria range 2, criteria 2…..)

first we give the col that needs to be summed(i.e quantity) and then the conditons.

![image.png](image%209.png)

### Q5. Avergae sale amount for each state.(AVERAGEIF)

=avergaeif(critriea range, ceirteira , avg range)

1. the col on which u want to apply the criteria ie. state for us
2. the condition 
3. the coll that needs to be avge ie. sales.

![image.png](image%2010.png)

### Q6. Average sale amount for each state and product name.

use  averageifs

![image.png](image%2011.png)

### Q7. cal ulate each city max sales. (MAXIFS)

![image.png](image%2012.png)