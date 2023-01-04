//# FizzBuzz
//Also used shift function( shifting value at -1 index, basically remove first element )

/**
 * @param {number} n
 * @return {string[]}
 */
var fizzBuzz = function(n) {
    const arr=[]
    for(let i=1 ; i<=n ;i++)
    {
        if(i % 3== 0 && i%5 == 0 )
        {
            arr[i]="FizzBuzz"
        }
        else if(i % 3== 0 && i % 5 != 0 )
        {
            arr[i]="Fizz"
        }
        else if(i % 3!= 0 && i % 5 == 0 )
        {
            arr[i]="Buzz"
        }
        else {
            arr[i] = `${i}`
        }
    }
    arr.shift();//It will shifting value on -1 index
    return arr;
};
