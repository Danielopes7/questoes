## 1
Complete the solution so that it returns true if the first argument(string) passed in ends with the 2nd argument (also a string).

Examples:
```
solution('abc', 'bc') // returns true
solution('abc', 'd') // returns false
```
**Result:**
```
function solution($str, $ending) {
    return str_ends_with($str, $ending);
}
```

## 2
Jaden Smith, the son of Will Smith, is the star of films such as The Karate Kid (2010) and After Earth (2013). Jaden is also known for some of his philosophy that he delivers via Twitter. When writing on Twitter, he is known for almost always capitalizing every word. For simplicity, you'll have to capitalize each word, check out how contractions are expected to be in the example below.

Your task is to convert strings to how they would be written by Jaden Smith. The strings are actual quotes from Jaden Smith, but they are not capitalized in the same way he originally typed them.

Example:

Not Jaden-Cased: "How can mirrors be real if our eyes aren't real";<br>
Jaden-Cased:     "How Can Mirrors Be Real If Our Eyes Aren't Real"

**Result:** 
```
function toJadenCase($string) 
{
  return ucwords( $string );
}
```

## 3
Create a function named divisors/Divisors that takes an integer n > 1 and returns an array with all of the integer's divisors(except for 1 and the number itself), from smallest to largest. If the number is prime return the string '(integer) is prime' (null in C#) (use Either String a in Haskell and Result<Vec<u32>, String> in Rust).

Example:
```
divisors(12); // => [2, 3, 4, 6]
divisors(25); // => [5]
divisors(13); // => '13 is prime'
```
**Result:** 

```
function divisors($integer) {
    $array = array();
    if ($integer == 1)
      return 0;
    for ($i = 2; $i <= $integer/2; $i++){
        if ($integer % $i == 0)
            array_push($array, $i);
    }
    if (!empty($array))
      return $array;
    return $integer. " is prime";
}
```
