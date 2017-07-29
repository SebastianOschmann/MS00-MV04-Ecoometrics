---
title       : Problem Set 1 - Introduction to R
description : Insert the chapter description here
--- type:NormalExercise lang:r xp:100 skills:1 key:deda7304f0

## Warm up and vectors I

##### Proposed editing time: < 5 min. 
##### Level: easy

Have a look at Task 1 a) from Problem Set 1. 

*** =instructions
Compute the following numbers with the corresponding R commands

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




--- type:NormalExercise lang:r xp:100 skills:1 key:8a0f1bc449

## Warm up and vectors III

##### Proposed editing time: < 5 min. 
##### Level: easy

Have a look at Task 1 c) and Task 1 d) from Problem Set 1. 

*** =instructions
Generate the vectors with the corresponding names from the Task 1 c) and compute XY


*** =hint



*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Generate a vector containing five ones
a <- 

# Generate a vector containing the sequence from one to ten
b <- 

# Generate a vector containg (1) the sequence from one to ten and (2) five ones 
c <-

# Multiply the vector a by 2 


# Compute the square root of the vector b


```

*** =solution
```{r}
a <- c(1,1,1,1,1)
b <- c(1,2,3,4,5,6,7,8,9,10)
c <- c(1,2,3,4,5,6,7,8,9,10, 1,1,1,1,1)
2*a
sqrt(b)
```

*** =sct
```{r}
test_object("a", incorrect_msg = "Attention, something is wrong with the vector a!")
test_object("b", incorrect_msg = "Attention, something is wrong with the vector b!")
test_object("c", incorrect_msg = "Attention, something is wrong with the vector c!")

test_output_contains("2*a", incorrect_msg = "A")
test_output_contains("sqrt(b)", incorrect_msg = "B")


test_error()
success_msg("Nice work!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:f23411b6a7
## Warm up and vectors IV

##### Proposed editing time: < 5 min. 
##### Level: medium

Consider the following vector: 

$$d = \frac{1} {(e^{28} + log(9))} \cdot [7 \; 1.5 \; 3 \; 4 \; 9]$$


*** =instructions
- Extract the third element of the vector d and store this element in i.

- Extract the the first two elements of the vector d and store this elements in ii.

- Extract the last element of the vector d and store this element in iii.

*** =hint
You can use square brackets to extract elements from a vector!


*** =pre_exercise_code
```{r}
d <- 1/(exp(28)+log(9))*c(7,1.5,3,4,9)
```

*** =sample_code
```{r}
# vector d has already been created
# Subtask i.
i <- 

# Subtask ii.
ii <- 

# Subtask iii.
iii <- 

```

*** =solution
```{r}
i   <- d[3]
ii  <- d[1:2]
iii <- d[5]


```

*** =sct
```{r}
test_object("i", incorrect_msg = "Attention, something is wrong with the vector i!")
test_object("ii", incorrect_msg = "Attention, something is wrong with the vector ii!")
test_object("iii", incorrect_msg = "Attention, something is wrong with the vector iii!")

test_error()
success_msg("Nice work!")
```



--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:34e0148626
## Matrices I

##### Proposed editing time: < 5 min. 
##### Level: medium


Have a look at the matrix C: 

$$C = 
\begin{bmatrix}
1 & 4 & 7 \newline
2 & 5 & 8 \newline
3 & 6 & 9
\end{bmatrix}$$  

Which command delivers the elements $1 \; 2 \; 3$?


*** =instructions
- C[1,2,3]
- C[1, ]
- C[ ,1]
- C[1]

*** =hint
You can use matrix[row,column] to extract elements from a matrix!


*** =pre_exercise_code
```{r}

```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 3)

```


--- type:PlainMultipleChoiceExercise lang:r xp:50 skills:1 key:dc47c431fc
## Matrices II

##### Proposed editing time: < 5 min. 
##### Level: medium


Have a look at the matrix D: 

$$D = 
\begin{bmatrix}
1 & 5 & 7 & 2 \newline
5 & 1 & 8 & 4 \newline
2 & 6 & 1 & 7 \newline
4 & 3 & 2 & 1
\end{bmatrix}$$  

Which command delivers the elements $2 \; 6 \; 1 \; 7$?


*** =instructions
- D[3 ]
- D[ ,3]
- D[3; ]
- D[3, ]

*** =hint
You can use matrix[row,column] to extract elements from a matrix!


*** =pre_exercise_code
```{r}

```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 4)

```



--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:2ed95de982
## Matrices III

##### Proposed editing time: < 5 min. 
##### Level: medium


Have a look at the matrix E: 

$$E = 
\begin{bmatrix}
3 & 2 & 1 & 9 \newline
4 & 9 & 2 & 1 \newline
1 & 6 & 1 & 7 \newline
4 & 7 & 6 & 4
\end{bmatrix}$$  


Which command delivers the number of all elements in matrix B?


*** =instructions
- length[E]
- E[?,?]
- E[rows+columns]
- E[rows, ] + E[ ,columns]

*** =hint
You can use matrix[row,column] to extract elements from a matrix, but you can not count rows and columns with this command.


*** =pre_exercise_code
```{r}

```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 1)

```




--- type:NormalExercise lang:r xp:100 skills:1 key:d6f26eda28
## Working with data frames I

##### Proposed editing time: < 10 min. 
##### Level: easy


Have a look at Task 3 a) from Problem Set 1. 



*** =instructions
- Generate the variable `bwgth_vec`. The variable contains the values of the birth weights. Store the results in `bwgth_vec`.

- Generate the variable `cigs_vec`. The variable contains the number of cigarettes smoked. Store the results in `bwgth_vec`.

*** =hint



*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Generate the vector bwght_vec
bwght_vec <- 

# Generate the vector cigs_vec
cigs_vec <- 

```

*** =solution
```{r}
bwght_vec <- c(109, 129, 104, 119, 115, 86, 139, 116, 126, 89)
cigs_vec  <- c(0, 6, 10, 20, 40, 0, 3, 30, 15, 40)
```

*** =sct
```{r}
test_object("bwght_vec", incorrect_msg = "Attention, something is wrong with bwght_vec!")
test_object("cigs_vec", incorrect_msg = "Attention, something is wrong with cigs_vec!")

test_error()
success_msg("Nice work!")
```



--- type:NormalExercise lang:r xp:100 skills:1 key:b8314b527f
## Working with data frames II

##### Proposed editing time: < 10 min. 
##### Level: medium


Have a look at Task 3 b) and c) from Problem Set 1. 

*** =instructions
- Match the vectors `bwght_vec` and `cigs_vec` to a matrix named `mat`. The first column should contain the birth weight and the second column should contain the number of cigarettes smoked. 
- Transform the matrix `mat` into a data frame and name it `data`.


*** =hint



*** =pre_exercise_code
```{r}
bwght_vec <- c(109, 129, 104, 119, 115, 86, 139, 116, 126, 89)
cigs_vec  <- c(0, 6, 10, 20, 40, 0, 3, 30, 15, 40)
```

*** =sample_code
```{r}
### The vectors "bwght_vec" and "cigs_vec" are already loaded in the workspace ###

# Create the matrix mat
mat <- 

# Transform the matrix mat into a data frame
data <- 

```

*** =solution
```{r}
mat <- cbind(bwght_vec, cigs_vec)
data <- data.frame(mat)
```

*** =sct
```{r}
test_object("mat", incorrect_msg = "Attention, something is wrong with the matrix mat!")
test_object("data", incorrect_msg = "Attention, something is wrong with the data frame!")

test_error()
success_msg("Nice work!")
```





--- type:NormalExercise lang:r xp:100 skills:1 key:a06d11695e
## Working with data frames III

##### Proposed editing time: < 5 min. 
##### Level: easy


Now, we want to learn how you can extract variables from a data frame.

*** =instructions
- Extract the birth weight variable from the data frame and store it in `bwght`.
- Extract the cigarettes variable from the data frame and store it in `cigs`.


*** =hint



*** =pre_exercise_code
```{r}
bwght_vec <- c(109, 129, 104, 119, 115, 86, 139, 116, 126, 89)
cigs_vec  <- c(0, 6, 10, 20, 40, 0, 3, 30, 15, 40)
mat <- cbind(bwght_vec, cigs_vec)
data <- data.frame(mat)
```

*** =sample_code
```{r}
### The data frame "data" is already loaded in the workspace ###

# Extract the birth weight variable and store it in "bwght"
bwght <-

# Extract the cigarettes variable and store it in "cigs"
cigs <- 


```

*** =solution
```{r}
bwght <- data$bwght_vec
cigs <- data$cigs_vec
```

*** =sct
```{r}
test_object("bwght", incorrect_msg = "Attention, something is wrong with the the variable "bwght"!")
test_object("cigs", incorrect_msg = "Attention, something is wrong with the  variable "cigs"!")

test_error()
success_msg("Nice work!")
```





--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:ca48b41f72
## Working with data frames IV

##### Proposed editing time: < 5 min. 
##### Level: medium

We want to learn more about birth weight. 

Therefore you must check the descriptive statistics of the variable bwght. The variable `bwght` is already loaded in the workspace.

What is the average birth weight?


*** =instructions
- 115.5
- 111.1
- 113.2
- 90.0


*** =hint
You can use the command `summary` to display descriptive statistics. 

*** =pre_exercise_code
```{r}
bwght <- c(109, 129, 104, 119, 115, 86, 139, 116, 126, 89)
```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 3)
```

