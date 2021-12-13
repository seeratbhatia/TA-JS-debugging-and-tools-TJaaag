### Write two tests for the following functions

#### Get full name### Write two tests for the following functions

#### Get full name

1. Write a function that takes two input `firstName` and `lastName` and returns full name. You will get the full name by adding first and last name with an space.
2. After writing the function write two tests for above function
3. Make the first test fail and look at the output
4. After making the first test fail do you see the output of the second test?

let fullName(firstName, lastName){
return fullName(firstName + lastName);
}
let result = fullname(firstName+""+lastName);
let expected = firstName lastName;

if (result !== expected){
throw New Error('${result} is not equal to ${expected}');
}
No it shows an error that firstNamelastName is not equal to firstName lastName.
#### Calculate total amount

1. Write a function that takes two input `amount` and `taxRate` and returns the total amount by `amount + (amount * taxRate) `
2. Write two tests for the above function
3. Make the first test fail and look at the output
4. After making the first test fail do you see the output of the second test?

let totalAmount(amount,taxRate){
return amount + (amount * taxRate);
}
let result = totalAmount(amount +(amount + taxRate));
let expected = amount + (amount * taxRate);

if(result !==expected){
throw New Error('${result} is not equal to ${expected}');
}
No it shows that both the value are not equal.

