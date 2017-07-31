---
title       : Problem Set 1 - Introduction to R
description : Insert the chapter description here
--- type:NormalExercise lang:r xp:100 skills:1 key:deda7304f0

## Task 1: Warm up and vectors I

##### Proposed editing time: < 5 min. 
##### Level: easy

Compute the following numbers: 

*** =instructions
- $\sqrt{798}$
- $|-9|$
- $10^3$
- $\sqrt{log(43)}$


*** =hint
Use the suggested functions.

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
# Use sqrt() to calculate the square root of 798
sqrt(798)

# Use abs() to calculate the absolute amount of - 9
abs(-9)

# Use "^" to calculate ten to the power of three
10^3

# Calculate the square root of the log of 43
sqrt(log(43))

```

*** =sct
```{r}
# Test objects

test_function("abs", incorrect_msg = "Something is wrong with the absolute amount of -9. Did you use: `abs( )`?")

test_output_contains("sqrt(798)", incorrect_msg = "Something is wrong with the square root of 798. Did you use: `sqrt( )`?")
test_output_contains("sqrt(log(43))", incorrect_msg = "Something is wrong with the square root of the log of 43")
test_output_contains("9", incorrect_msg = "Something is wrong with the absolute amount of -9!")
test_output_contains("1000", incorrect_msg = "Something is wrong with ten to the power of three!")

test_error()
success_msg("Nice work!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:df487377ba

## Task 1: Warm up and vectors II

##### Proposed editing time: < 5 min. 
##### Level: easy

Have a look at Task 1 b) from Problem Set 1. 

*** =instructions
Generate the variables with the corresponding variable names from the Task 1 b)!


*** =hint
Hint fehlt noch!

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Generate the variable u
u <- 

# Generate the variable v
v <- 

# Generate the variable w 
w <- 

# Generate the variable x 
x <- 

# Generate the variable y 
y <- 

# Generate the variable z
z <- 

```

*** =solution
```{r}
# Generate the variable u
u <- 10.5
 
# Generate the variable v
v <- 2

# Generate the variable w 
w <- 3*u+v

# Generate the variable x 
x <- 3*(u+v)

# Generate the variable y 
y <- (3*u)+v

# Generate the variable z
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

## Task 1: Warm up and vectors III

##### Proposed editing time: < 10 min. 
##### Level: easy

Generate the following vectors with the corresponding names!


*** =instructions
- $a \, = [1 \; 1 \; 1 \; 1 \; 1]$ 
- $b \, = [1 \; 2 \; 3 \; 4 \; 5 \; 6 \; 7 \; 8 \; 9 \; 10]$
- $c \, = [1 \; 2 \; 3 \; 4 \; 5 \; 6 \; 7 \; 8 \; 9 \; 10 \; 1 \; 1 \; 1 \; 1 \; 1]$
- Compute: $2 \cdot b$
- Compute: $\sqrt{b}$


*** =hint



*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Generate the vector a 
a <- 

# Generate the vector b
b <- 

# Generate the vector c
c <-

# Multiply the vector b by 2 


# Compute the square root of the vector b


```

*** =solution
```{r}
# Generate the vector a 
a <- c(1,1,1,1,1)

# Generate the vector b
b <- c(1,2,3,4,5,6,7,8,9,10)

# Generate the vector c
c <- c(1,2,3,4,5,6,7,8,9,10, 1,1,1,1,1)

# Multiply the vector b by 2 
2*a

# Compute the square root of the vector b
sqrt(b)

```

*** =sct
```{r}
test_object("a", incorrect_msg = "Attention, something is wrong with the vector a!")
test_object("b", incorrect_msg = "Attention, something is wrong with the vector b!")
test_object("c", incorrect_msg = "Attention, something is wrong with the vector c!")

test_output_contains("2*a", incorrect_msg = "Attention, something is wrong with the computation of `2*b`")
test_output_contains("sqrt(b)", incorrect_msg = "Attention, something is wrong with the computation of `sqrt(b)`")


test_error()
success_msg("Nice work!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:f23411b6a7
## Task 1: Warm up and vectors IV

##### Proposed editing time: < 5 min. 
##### Level: medium

Consider the following vector: 

$$d = \frac{1} {(e^{28} + log(9))} \cdot [7 \; 1.5 \; 3 \; 4 \; 9]$$


*** =instructions
- Extract the third element of the vector d and store this element in i!

- Extract the the first two elements of the vector d and store this elements in ii!

- Extract the last element of the vector d and store this element in iii!

*** =hint
You can use square brackets to extract elements from a vector!


*** =pre_exercise_code
```{r}
d <- 1/(exp(28)+log(9))*c(7,1.5,3,4,9)
```

*** =sample_code
```{r}
### vector d has already been created ###

# Subtask i
i <- 

# Subtask ii
ii <- 

# Subtask iii
iii <- 

```

*** =solution
```{r}
### vector d has already been created ###

# Subtask i
i   <- d[3]

# Subtask ii
ii  <- d[1:2]

# Subtask iii
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
## Task 2: Matrices I

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

The matrix is loaded in the workspace and named `C`. You can use the R Console on the right side to test the commands!



*** =instructions
- C[1,2,3]
- C[1, ]
- C[ ,1]
- C[1]

*** =hint
- You can use matrix[row,column] to extract elements from a matrix!


*** =pre_exercise_code
```{r}
C <- cbind(c(1,2,3), c(4,5,6), c(7,8,9))
```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 3)

```


--- type:PlainMultipleChoiceExercise lang:r xp:50 skills:1 key:dc47c431fc
## Task 2: Matrices II

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
## Task 2: Matrices III

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

The matrix is loaded in the workspace and named `E`. You can use the R Console on the right side to test the commands!

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
E <- cbind(c(3,4,1,4), c(2,9,6,7), c(1,2,1,6), c(9,1,7,4))
```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 1)

```




--- type:NormalExercise lang:r xp:100 skills:1 key:d6f26eda28
## Task 3: Working with data frames I

##### Proposed editing time: < 10 min. 
##### Level: easy


Have a look at Task 3 a) from Problem Set 1. 



*** =instructions
- Generate the variable `bwgth_vec`. The variable contains the values of the birth weights. Store the results in `bwgth_vec`.

- Generate the variable `cigs_vec`. The variable contains the number of cigarettes smoked. Store the results in `bwgth_vec`.

*** =hint
- You can use `c` to combine values into a vector or list! 


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
# Generate the vector bwght_vec
bwght_vec <- c(109, 129, 104, 119, 115, 86, 139, 116, 126, 89)

# Generate the vector cigs_vec
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
## Task 3: Working with data frames II

##### Proposed editing time: < 10 min. 
##### Level: medium


The vectors `bwght_vec` and `cigs_vec` are already loaded in the workspace. 

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
### The vectors "bwght_vec" and "cigs_vec" are already loaded in the workspace ###

# Create the matrix mat
mat <- cbind(bwght_vec, cigs_vec)

# Transform the matrix mat into a data frame
data <- data.frame(mat)

```

*** =sct
```{r}
test_object("mat", incorrect_msg = "Attention, something is wrong with the matrix!")
test_object("data", incorrect_msg = "Attention, something is wrong with the data frame!")

test_error()
success_msg("Nice work!")
```





--- type:NormalExercise lang:r xp:100 skills:1 key:a06d11695e
## Task 3: Working with data frames III

##### Proposed editing time: < 5 min. 
##### Level: easy


Now, we want to learn how you can extract variables from a data frame. The data frame `data` is already loaded in the workspace. 


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
### The data frame "data" is already loaded in the workspace ###

# Extract the birth weight variable and store it in "bwght"
bwght <- data$bwght_vec

# Extract the cigarettes variable and store it in "cigs"
cigs <- data$cigs_vec

```

*** =sct
```{r}
test_object("bwght", incorrect_msg = "Attention, something is wrong with the the variable `bwght`!")
test_object("cigs", incorrect_msg = "Attention, something is wrong with the  variable `cigs`!")

test_error()
success_msg("Nice work!")
```





--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:ca48b41f72
## Task 3: Working with data frames IV

##### Proposed editing time: < 5 min. 
##### Level: medium

We want to learn more about the birth weight. Therefore you can check the descriptive statistics of the variable `bwght`. The variable `bwght` is already loaded in the workspace. So you can use the R Console on the right side. 

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





--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:21f224e94c
## Task 3: Working with data frames V

##### Proposed editing time: < 5 min. 
##### Level: very easy

Obviously you are able to work with the R Console. Than I have a very easy question:

What is the minimum birth weight (variable `bwght`)?


*** =instructions
- 86.0
- 14.2
- 92.9
- 105.2


*** =hint
You can use the command `summary` to display descriptive statistics. 

*** =pre_exercise_code
```{r}
bwght <- c(109, 129, 104, 119, 115, 86, 139, 116, 126, 89)
```

*** =sct
```{r}
msg_success <- "Exactly!"
test_mc(correct = 1)
```





--- type:NormalExercise lang:r xp:100 skills:1 key:e0afb176ef
## Task 5: Random number generation

##### Proposed editing time: < 10 min. 
##### Level: medium

At least, we want to learn something about random number generation. 


*** =instructions
- Generate `x` according to $x_i \sim N(0,9), i = 1,...,50$. It is very important, that you use `set.seed(123)` before generating the numbers. Otherwise we can not check your result.
- Compute the mean, the variance and the standard deviation of `x` with the according commands.


*** =hint
- You can generate random variables with `rnorm(n, mean = ?, sd = ?)`

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Do not forget to use set.seed


# Store the random numbers in "x"
x <- 

# Compute the mean of x


# Compute the variance of x


# Compute the standard deviation of x


########################################
#   Do not change the following line!  #
# With this line we check your results #
########################################
y <- round(sum(x), 2)

```

*** =solution
```{r}
# Do not forget to use set.seed
set.seed(123)

# Store the random numbers in "x"
x <- rnorm(50, mean = 0, sd = 3)

# Compute the mean of x
mean(x)

# Compute the variance of x
var(x)

# Compute the standard deviation of x
sd(x)

########################################
#   Do not change the following line!  #
# With this line we check your results #
########################################
y <- round(sum(x), 2)
```

*** =sct
```{r}
test_object("y", incorrect_msg = "Attention, something is wrong with the random number generation!")

test_output_contains("mean(x)", incorrect_msg = "Did you compute the mean of x with the according command?")
test_output_contains("sd(x)", incorrect_msg = "Did you compute the standard deviation of x with the according command?")
test_output_contains("var(x)", incorrect_msg = "Did you compute the variance of x with the according command?")

test_error()
success_msg("Nice work!")

```
