---
title       : Problem Set 1 - Introduction to R
description : Insert the chapter description here
--- type:NormalExercise lang:r xp:100 skills:1 key:deda7304f0

## Warm up and vectors I

##### Proposed editing time: < 5 min. 
##### Level: easy

Have a look at Task 1 a) from Problem Set 1. 

*** =instructions
Compute the following numbers with the corresponding R commands and store the results in the associated vector.

*** =hint
Und das steht unter hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Use sqrt() to calculate the square root of 798


# Use abs() to calculate the absolute amount of - 9


# Use "^" to calculate ten to the power of three


# Calculate the square root of the log of 43


```

*** =solution
```{r}
# Calculate the square root of 798 and store the result in i
sqrt(798)

# Calculate the absolute amount of - 9 and store the result in ii
abs(-9)

# Calculate ten to the power of three and store the result in iii
10^3

# Calculate the square root of the log of 43 and store the result in iv
sqrt(log(43))

```

*** =sct
```{r}
# Test objects
test_function("sqrt", incorrect_msg = "Something is wrong with the square root of 798. Did you use: sqrt( )?")
test_function("abs", incorrect_msg = "Something is wrong with the absolute amount of - 9. Did you use: abs( )?")
test_function("^", incorrect_msg = "Something is wrong with ten to the power of three. Did you use: ^ ?")
test_error()
success_msg("Nice work!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:df487377ba

## Warm up and vectors II

##### Proposed editing time: < 5 min. 
##### Level: easy

Have a look at Task 1 b) from Problem Set 1. 

*** =instructions
Generate the variables with the corresponding variable names from the Task 1 b)


*** =hint

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Generate the variable u which contains 10.5
u <- 

# Generate the variable v which contains 2
v <- 

# Generate w 
w <- 

# Generate x 
x <- 

# Generate y 
y <- 

# Generate z
z <- 

```

*** =solution
```{r}
u <- 10.5
v <- 2
w <- 3*u+v
x <- 3*(u+v)
y <- (3*u)+v
z <- exp(2.5+v)
```

*** =sct
```{r}
# Test objects
test_object("u", incorrect_msg = "Attention, something is wrong with the variable u!")
test_object("v", incorrect_msg = "Attention, something is wrong with the variable v!")
test_object("w", incorrect_msg = "Attention, something is wrong with the variable w!")
test_object("x", incorrect_msg = "Attention, something is wrong with the variable x!")
test_object("y", incorrect_msg = "Attention, something is wrong with the variable y!")
test_object("z", incorrect_msg = "Attention, something is wrong with the variable z!")

test_error()
success_msg("Nice work!")
```



