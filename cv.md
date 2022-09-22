# Xeniya Gazizova
## Contacts
* *Location:* Merced, California, USA
* *Phone:* +1(209)5048901
* *Telegram:* @xeniya_mv
* *E-mail:* xeniya.gazizova@gmail.com

## About me

## Education
* **Bachelor's Degree.** Lomonosov Moscow State University. Field of study - Mathematics. Period of education - 2015-2019.

## Courses
* [JavaScript, part 1.](https://www.coursera.org/learn/javascript-osnovy-i-funktsii)

![Coursera course 1](/images/coursera_js_1.png)

* [HTML, CSS, and Javascript for Web Developers.](https://www.coursera.org/learn/html-css-javascript-for-web-developers)

![Coursera course 2](/images/coursera_html_css_js.png)

## Skills
* **C/C++**

*The main programming languages at the university. Basic knowledge.*
* **Python(Libraries: NumPy, SciPy, Pandas)**

*Used for final project at the university and some common tasks at work*
* **JavaScript**

*Basic knowledge*
* **CSS3**

*Basic knowledge*
* **HTML5**

*Basic knowledge*
* **Git/GitHub**
* **Teradata SQL**
* **Hue (Hadoop User Experience)**

## Work experience
* Place of work: [Sber](www.sberbank.ru)
    - *12.11.2020 - 01.02.2021* - Intern
    - *02.02.2021 - 22.10.2021* - Data analyst
* Experience:
    - Developed an algorithm for aggregating geolocation data from the bank's mobile application using PySpark. It increased the quality of AI model - R2 by 12%.
    - Prepared data for 7 different AI bank models. The effect of these AI models reaches $50 million.
    - Scored over 90 million customers by PySpark for the likelihood of opening a small business bank account.
    - Prepared data for automatic validation of 11 ML models.


## Code example
* *Kata:* Roman Numerals Decoder
* *Description:* Create a function that takes a Roman numeral as its argument and returns its value as a numeric decimal integer. You don't need to validate the form of the Roman numeral.
* *Example:*
```
solution('XXI'); // should return 21

```
* *Solution:*
```
function solution (roman) {
    var romanNumbersValues = {
        'I': 1,
        'V': 5,
        'X': 10,
        'L': 50,
        'C': 100,
        'D': 500,
        'M': 1000
    };

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
[coursera_html_css_js](https://github.com/XeniyaMV/coursera_html_css_js) is my GitHub repository with solutions for  [HTML, CSS, and Javascript for Web Developers course from Coursera](https://www.coursera.org/learn/html-css-javascript-for-web-developers).

## Languages
* Russian - Native
* English - Upper-intermediate/Advanced. English level was checked by [EFSET](https://www.efset.org/ef-set-50/).
See [English level certificate](/images/EF%20SET%20Certificate.pdf).
