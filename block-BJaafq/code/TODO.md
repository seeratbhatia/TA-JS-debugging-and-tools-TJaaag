
#### Write your implementation of testing framework and assertion. Only after completing this go forward.
testing framework:

function test(message,callback){
    try{
        callback();
        console.log('✅',message); 
    }catch(error){
        console.error(error);
        console.log('❌', message);
    }
}

framework assertion:

function expect(actual){
    return{
        to equal : function (expected){
            if (actual !== expected){
                throw new error('${actual} is not equal to ${expected}');
            }
        }
    }
}
#### Write two tests for the following functions using test framework assertion

#### Add two number

1. Write a function that takes two input `numA` and `numB` and returns the sum of both numbers.
2. After writing the function write 5 tests for above function with different values
3. Throw an error when the arguments passed in not a number.
4. Make first test fail and see if you get the result of second test.
5. If not fix it using the test framework (try...catch) we learned in the testing framework video.


function expect(actual){
    return{
        to equal : function (expected){
            if (actual !== expected){
                throw new error('${actual} is not equal to ${expected}');
            }
        }
    }
}
function testAdd(){
    result = add(numA + numB);
    expected = numA+numB;
    expect (result). to equal (expected);
}

#### Multiply two numbers

1. Write a function that takes two input `numA` and `numB` and returns the multiplication of both numbers.
2. After writing the function write 5 tests for above function with different values
3. Throw an error when the arguments passed in not a number.
4. Make first test fail and see if you get the result of second test.
5. If not fix it using the test framework (try...catch) we learned in the testing framework video.

function expect(actual){
    return{
        to equal : function (expected){
            if (actual !== expected){
                throw new error('${actual} is not equal to ${expected}');
            }
        }
    }
}
function testAdd(){
    result = add(numA * numB);
    expected = numA*numB;
    expect (result). to equal (expected);
}
