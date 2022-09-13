# Xeniya Gazizova
## Contacts
* *Location:* Merced, California, USA
* *Phone:* +1(209)5048901
* *Telegram:* @xeniya_mv
* *E-mail:* xeniya.gazizova@gmail.com
## About me
## Education
* **Bachelor Degree.** Lomonosov Moscow State University. Field of study - Mathematics. Period of education - 2015-2019.
## Courses
## Skills
* C/C++
* Python
* JavaScript
* CSS3
* HTML5
* Git/GitHub
* Teradata SQL
## Work experience
## Code example
* *Kata:* Roman Numerals Decoder
* *Description:* Create a function that takes a Roman numeral as its argument and returns its value as a numeric decimal integer. You don't need to validate the form of the Roman numeral.
* *Example:*
```
solution('XXI'); // should return 21

```
* *Solution:*
```
var romanNumbersValues = {
    'I': 1,
    'V': 5,
    'X': 10,
    'L': 50,
    'C': 100,
    'D': 500,
    'M': 1000
};

function solution (roman) {
    // complete the solution by transforming the
    // string roman numeral into an integer
    var givenRomanNumber = roman.split('');
    var intNumbers = [];
    var res = 0;
  
    for (var i = 0; i < givenRomanNumber.length; i++) {
        intNumbers.push(romanNumbersValues[givenRomanNumber[i]]);
    };
  
    if (intNumbers.length == 1) {
        return intNumbers[0];
    }

    for (var i = intNumbers.length - 1; i >= 0; i--) {
        if (i == 0 && intNumbers[i] >= intNumbers[i+1]) {
            res += intNumbers[i];
        }
        else if (i != 0) {
            if (intNumbers[i] > intNumbers[i-1]) {
                res += intNumbers[i] - intNumbers[i-1]
                i--;
            }
            else {
                res += intNumbers[i];
            }
        }
    }
    return res;

};

```

## Projects
## Languages
* Russian - Native
* English - Intermediate/Upper-intermediate. English level was checked by [https://www.efset.org/quick-check/][EFSET]