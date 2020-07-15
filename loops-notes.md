
# comparison
- **comparison**:-is evaluate a situation by comparing one value in the script to whatyou expect it might be. the resalt will be a boolean:**true or false**.

1. ```==``` is equalto :- compares two values ```(numbers,strings,booleans)``` to see if they are the same.

- example:- ```'Hello' == 'Goodbye'``` retuns false. they are not the same string.

- ```'Hello' == 'Hello'``` returns true. they are the same string.

2. ```!=``` is not equal:-compares two values ```(numbers,strings,booleans)``` to see if they are not the same.

- example:- ```'Hello'!= 'Goodbye'``` returns true. they are note the same string.

- ```'Hello' != 'Goodbye'``` returns false. they are the same string.

3. ```===``` strict equal to:- compare two values to check that both the data type and value **are the same**.

- example:- ```'3' === 3``` returns false. tehy are not the same data type or value.

- ```'3' === '3'``` returns true. they are the same data type and value.

4. ```!==``` strict not equal to :-compare two values to check that both the data type and value **are not the same**.

- example:- ```'3' !== 3``` returns **true**. because there are not the same data type.

- ```'3' !== '3'``` returns **false**.because there are the same data type.


# LOOPS
- check a condition. if it returns true,a code block will run.then the condition will be cvhecked again and if it still retuens true, the code block will run again.it repeats until the condition returns false.

### there are three common types of loops:

- **FOR LOOPS**:-if you need torun code a specific number of times.the condition is usually a counter.

- **WHILE LOOPS**:-if you do not know how many times the code should run.condition can be something other than a counter.

- **DO LOOPS**:-this loop is very similar to while loops.but has one key diffrence it will be always run the statments inside the curly braces at least once,even if the condition evaluation to false.

- for loop example:- ```for (var i=0; i <10; i++){```
                           ```document.write(i);```
                           ```}```

- For Loop usea a counter as a condition.this instructs the code to run a specified of times,the condition is made up of three statments:

1. Intialization:- creat a variable and set it to 0,this variable is commonly called i.and acts as the counter.
   ```var i= 0;```

2. condition:-the loop should continue to run antil the number reaches a spesified number. ```i < 10;```

3. update:-every time the loop has run the statmentes in the curly braces,its adds one to the count number. ```i++```