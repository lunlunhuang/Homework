## (1.)
  -  _prefix free_ code : 1 , 4 <br>
   
   - decision tree of code1 :<br>
   
   - decision tree of code4 :<br>

## (2.)

  (a)<br>
  (b)

  |title|_s<sub>1</sub>_|_s<sub>2</sub>_|_s<sub>3</sub>_|_s<sub>4</sub>_|_s<sub>5</sub>_|_s<sub>6</sub>_|_s<sub>7</sub>_|
  |:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
  |_p(x)l(x)_|0.5|0.5|0.375|0.375|0.375|0.25|0.25|
  |_l(x)_|2|2|3|3|3|4|4|
  |_c(x)_|00|01|100|101|110|1110|1111|
  |_p(x)_|0.25|0.25|0.125|0.125|0.125|0.0625|0.0625|
  |      |     |     |     |     |     |  0\ | /1  |
  |      |     |     |     |     |     |0.125|     |
  |      |  0\ | /1  |  0\ | /1  |  0\ | /1  |     |
  |      | 0.5 |     | 0.25|     | 0.25|     |     |
  |      |     |     |  0\ |     |  /1 |     |     |
  |      |     |     | 0.5 |     |     |     |     |
  |      |  0\ |     | /1  |     |     |     |     |
  |      |     | 1.0 |     |     |     |     |     |

  (c) <br>
  
  L = 0.25 * 2 + 0.25 * 2 + 0.125 * 3 + 0.125 * 3 + 0.125 * 3 + 0.0625 * 4 + 0.0625 * 4 <br>
      = 0.5 + 0.5 + 0.375 + 0.375 + 0.375 + 0.25 + 0.25 <br>
      = 2.625<br>
      
  average code length = 2.625 / 7 <br>
                      = 0.375 <br>

  (d)<br>
  
  

## (3.)

- sourse : abcabcabcabcabcabcabcabcabcabcabcabc <br>

- encode : 
|Current|Next|Output|Add to dictionay|Comments|
|:---:|:---:|:---:|:---:|:---|
|a 97|b 98|a 97|ab 256|'ab' not exist, add it to table|
|b 98|b 98|b 98|bb 257|'bb' not exist, add it to table|
|b 98|b 98|-|-|'bb' exist in table, 'bba' not exist|
|bb 257|a 97|bb 257|bba 258|add 'bba' to table|
|a 97|b 98|-|-|'ab' exist in table, 'abb' not exist|
|ab 256|b 98|ab 256|abb 259|add 'abb' to table|
|b 98|b 98|-|-|'bb' exist in table, 'bba' exist to, 'bbab' not|
|bba 258|b 98|bba 258|bbab 260|add 'bbab' to table|
|b 98|-|b 98|-|end|

-code :













