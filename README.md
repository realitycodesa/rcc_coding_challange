# Task

- Parse `data.json` into the query similar to `result.sql`. Video Explaining the task [HERE](https://drive.google.com/file/d/1VMeqR9xavh-cpEIbhi2DU6ZipqoUwSY5/view?usp=sharing)

- Inside `data.json` you have two properties `nodes` and `edges`, `nodes` contains all the required
information to apply the transformation into Query and `edges` represents how they are linked together. In each node there is a property `transformObject` which is different for each `type`

- There are 5 different types of nodes used in this request

   - INPUT		                --> it contains information about table and which fields to select from original table. 
   - FILTER	                    --> contains SQL "where" settings 
   - SORT		                --> contains SQL "order by" settings 
   - TEXT_TRANSFORMATION	    --> contains information about applying some text SQL function on any column. For example UPPER, LOWER (see the digram for actual use case)
   - OUTPUT	                    --> contains SQL "limit" settings

Graphical representation of actual use-case:

![graphical representation](https://github.com/goes-funky/modeling-test/blob/master/graphical-representation.png?raw=true) 


- Include unit testing for every transformation
- include a dockerfile to deploy and test your solution


Use your imagination to fill in the missing information however you like to achieve the result.

# Bonus Points
 - Optimize `data.json` json structure/schema.
 - Extendable structure which allows to add more types easily in the future.
