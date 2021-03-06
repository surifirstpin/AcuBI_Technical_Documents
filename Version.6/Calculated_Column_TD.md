


<center><h1>Calculated Column</h1></center>

Calculated Column allows user to manipulate the retrieved data using arithmetical, logical, text-based and date-based functions and displays the same in required format. The data extracted using calculated column will show up in green colour in the data table. Just like regular dimensions and measures, calculated columns are controlled from display in visualizations.

### Functionalities of Calculated Column

- It supports wide variety of arithmetical and logical operations, to be applied on the data.

- Perform calculation, using data from external parameters (through "Global parameters") using reference to the database fields. 

- It controls or access the data with user wise calculations.

-  Optimize and transform the data using  <b>#plugin#</b>  functionality.

- Define a function or use a global function to be applied on the required data fields.
 
> **Note:** The functions support JavaScript API.

### Deriving Expression

Click on <b>Calculated column</b> button to enable table calculations as shown in below image,

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/8449a0efb0dbe441c6e7ce6e6db2093f5a3afd7c/images/New_version5/TD_CC_Image0.png)

<b><font color = "Black"> Image 1</b>

After navigating to Calculated Column Window, Enter all the below fields.

- <b>Field name</b> unique identifier name to refer calculated column.

- <b>Label</b> labeling the calculated column.

- <b>Data Type</b> data type used (string,number).

- <b>Field Type </b>derives dimension or measure.

- <B>Calculation</b> To derive a expressions, enter $ symbol in calculation window, it will display list of functions and fields available for executing arithmetical & logical expressions in calculated column section or else you can choose your functionality manually by selecting the suitable functions available on right side of the screen.

- <b>Calculate on the raw data</b> this function is applied directly on the retrieved value of the fields, initially before pivot or grouping options are applied.

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/4ae4c6efd84be04af3ef553c09572728d221d5e1/images/New_version5/TD_CC_Image1.png)

<b><font color = "Black"> Image 2</b>

- Click <b>OK</b> after deriving the expression,  all the values based on calculation is shown up in green color as shown in below image,

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/b8aa0f8eae4b1049cbad5181768151ac000c92c7/images/New_version5/TD_CC_Image2.png)

<b><font color = "Black"> Image 3</b>

## Mathematical operation 

Custom made mathematical operations can be added in calculated column section as shown in below Image;

<b>Example 1 :</b>

 To calculate <b>Number of working days</b> in each month, use the below expression in calculation field window as shown in below image; 

```
bi.days_in_month(${biplus.orders.whenmade} )
```

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/aa7e1c3a36eeb11f25ad5875fc8ce06f343b0a4c/images/New_version5/TD_CC_Image4.png)

 <b><font color = "Black"> Image 4</b>
 
 
The resultant for this calculated column will display number of working days in each month.
 
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/31694b27949602c0eddb042edb970497f11b2b5f/images/New_version5/TD_CC_Image5.png)

<b><font color = "Black"> Image 5</b>

<b><i><u>AcuBi supports following functionalities in calculated column;</u></i></b>

### General

| Name| Description  | Usage and  Example|
|--|--|--|
|<b>Offset</b>  |Return the row value of the column mentioned as before or after based on  -Ve or +Ve number given  | bi.offset(#{col_name}, row_difference) |
|<b>pivot_offset</b>|Returns the cell value of pivot table based on the Row and Column position given respectively.Row number:  +Ve & -Ve are for below & above positions Column number : +Ve and -Ve are for after & before positions|bi.pivot_offset(#{col_name} ,m,n) for instance: m is row number & n is column number|
|<b>Contains</b>|Returns true/ false after validating expression given inside|bi.contains(expression)|
|<b>row_total</b>|Returns the total value in the row for the preceding measures (before the present column) |bi.row_total ( )|
|<b>col_total</b>|Returns the total value of the column given inside ()|bi.column_total(#{col_name})|
|<b>number</b>|Returns the object argument to a number that represents the object's value.The object may be static or a column name|bi.number(“static”) or bi.number(${col_name}) Ex: bi.number("1234567") returns  1234567|
|<b>int</b>|Returns only integer values of given number or column|bi.int(number) or bi.int(${col_name})Ex: bi.int(74845.9898) = 74845|
|<b>in_globals</b>|Returns the data from Global parameters based on the common reference. The reference can be static or a column|bi.in_globals(Ref ,”GP_Name.R_Val ”, ”Ref_key” ) **Note:** Ref can be a column name or static value or userid|
|<b>in_global_key</b>|it returns the data from global parameters based on the multiple common references.this references can be static or column|bi.in_global_keys ([“GP_Rkey1”,”GP_Rkey2”,.....],[Ref1, Ref2,.....], ”GP_Name.R_Val”) Note: Ref1/Ref2 can be static strings or column names or userid|
|<b>calculate_key_group</b>|Returns an aggregated value of a measure based on a dimension with further mention of row grouping column name|bi.calculate_key_group (#Ag_col,$Ag_col,#RG_col,$RG_col,$M_col,”agg_type”) Where Ag= Aggregated & RG for Row Grouping  & M_Col for measure and agg_type can be sum, avg, min, max, count|
|<b>col_running_total</b>|Returns the running total value for a column in each cell|bi.col_running_total(#{col_name})|
|<b>col_running_avg</b>|Returns the average value upto current cell for a column|bi.col_running_avg(#{col_name})|

### Statistics

|  Name | Description | Usage & Example|
|  :------: | :------: | :------: |
|  <b>unequal</b> | Returns true / false if the inputs given are not equal. | bi.unequal(m,n)<br/>Returns true if m=n else false |
|  <b>mad</b> | Returns the Median Absolute Deviation for the inputs | bi.mad(p1,p2,p3,......)<br/>Ex: bi.mad(100,200) = 50 |
|  <b>max</b>| Returns the maximum value of a matrix or a list with values. | bi.max(p1,p2,p3,.....)<br/>Ex: bi.max(100,200,300) = 300 |
|  <b>mean</b> | Returns the mean value of a list of values mentioned | bi.mean(p1,p2,p3)<br/>Ex: bi.mean(100,200,300) = 200 |
|  <b>median</b> | Returns the median value of a list of values mentioned | bi.median(p1,p2,p3,.....) |
|  <b>mode </b>| Returns the values which are repeated in the list mentioned | bi.mode(p1,p2,p3,.....)<br/>Ex: bi.mode(1,2,1)=1 |
|  <b>prod</b>| Returns the product values of the mentioned values |bi.prod(p1,p2,p3,p4,....) Ex: bi.prod(p1,p2,p3) = p1 * p2 * p3|
|  <b>quantileSeq</b> | Returns prob order quantile of a matrix or a list with values | bi.quantileSeq(A, prob[, sorted]) |
|  <b>std</b> | Returns the standard deviation of a matrix or a list with values. | bi.std(p1,p2,p3 ...)<br/>bi.std(A)<br/>bi.std(A, normalization) |
|  <b>sum</b> | Returns the sum of list of values mentioned | bi.sum(p1,p2,p3,.....)<br/>Ex: bi.sum(p1,p2,p3) = p1 + p2 +p3 |
|  <b>var</b> | Returns the variance of a matrix or a list with values | bi.var(p1,p2,p3)<br/>Ex: bi.var(2, 4, 6) = 4 |

### Date

|  Name | Description | Usage & Example |
|  :------: | :------: | :------: |
|  <b>date_to_week</b> | Returns the week number in the year for the date given | bi.date_to_week(${col_name})<br/>Ex: bi.date_to_week(“2018-02-11”) = 7 |
|  <b>date_to_month</b> | Returns the month number in the year for the date given | bi.date_to_month(${col_name})<br/>Ex: bi.date_to_month(“2018-02-11”) = 2 |
|  <b>date_to_quarter</b> | Returns the quarter number in the year for the date given | bi.date_to_quarter(${col_name})<br/>Ex: bi.date_to_quarter(“2018-02-11”) = 1 |
|  <b>date_to_year</b> | Returns the year for the date given | bi.date_to_year(${col_name})<br/>Ex: bi.date_to_year(“2018-02-11”) = 2018 |
|  <b>date_format</b> | Returns the required format (supported by the database) of a date given |bi.date_format(${col_name}, “required_format”) Ex: bi.date_format(“2018-02-10 235950”, “YYYY-MM”) = 2018-02 |
| <b>date_diff</b> | Returns the number of days between two given dates | bi.date_diff(date1,date2) |
| <b>days_in_month</b> | Returns the total number of days in a month for a given date / time stamp | bi.days_in_month (${Col_name}) Ex: bi.days_in_month(“2018-02-01 15:32:26”) = 28 |
| <b>days_till_month</b> | Returns the total number of days completed in a month for a given date / time stamp | bi.days_till_month (${Col_name})Ex: bi.days_in_month(“2018-02-01 15:32:26”) = 1 |

### Bitwise Operator

|  **Name** | **Description** | **Usage & Example** |
|  :------: | :------: | :------: |
|  <b>bitAnd</b> | Bitwise AND two values, x & y. Ex. bit And(x, y) | bi.bitAnd(53, 131) = 1 |
|  <b>bitNot</b> | Bitwise NOT value, ~x. | bi.bitNot(1) = -2, <br/>bi.bitNot([2,-3,4]) = [-3,2,5] |
|  <b>bitOr</b> | Bitwise OR two values, x&#124 y.| bi.bitOr(1,2) = 3, <br/>bi.bitOr([1,2,3],4) = [5,6,7] |
|  <b>bitXor</b> | Bitwise XOR two values, x ^ y. | bi.bitXor(1, 2) = 3, <br/>bi.bitXor([2, 3, 4], 4) = [6,7,0] |
| <b> leftShift</b> | Bitwise left logical shift of a value x by y number of bits, x << y. | bi.leftShift(1, 2) = 4, <br/>bi.leftShift([1, 2, 3], 4) = [16, 32, 64] |
| <b> rightArithShift</b> | Bitwise right arithmetic shift of a value x by y number of bits, x >> y. | bi.rightArithShift(4, 2) = 1, <br/>bi.rightArithShift([16, -32, 64], 4) = [1, -2, 3] |
|  <b>rightLogShift</b> | Bitwise right logical shift of value x by y number of bits, x >>> y. | bi.rightLogShift(4, 2) = 1, <br/>bi.rightLogShift([16, -32, 64], 4) = [1, 2, 3] |

### Arithmetic

|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>abs</b> | Returns the absolute value of a number<br/>It removed the -ve symbol for a negative value and displays the result as positive value | bi.abs(${Col_name})<br/>Ex: bi.abs(-2) = 2 |
|  <b>add</b> | Returns the value which obtained by adding the given list of values | bi.add(p1,p2,p3,.....)<br/>Ex: bi.add(3,4) = 7 |
|  <b>cbrt</b> | Returns the cuberoot value  of a give value | bi.cbrt(value)<br/>Ex: bi.cbrt(27) = 3 |
|  <b>ceil</b> | Returns the smallest integer greater than or equal to the given number | bi.ceil(value)<br/>Ex: bi.ceil(3.1) = 4 & bi.ceil(-8.5) = -8 |
|  <b>cube</b> | Returns the cube value of given value | bi.cube(value)<br/>Ex: bi.cube(3)=27 |
|  <b>divide</b> | Return the results after divides the two given values | bi.divide(m,n) = m/ n<br/>Ex: bi.divide(6,3) = 2 |
|  <b>fix</b> | Round the integer value for a given value towards zero. | bi.fix(value)<br/>Ex: bi.fix(4.5) = 4, fix(-4.5) = -4 |
|  <b>floor</b> | Round the integer value for given value towards minus infinity. | bi.floor(value)<br/>Ex: floor(2.8) = 2, floor(-7.5) = -8 |
|  <b>dotDivide</b> | Returns the value obtained after dividing two matrices element wise | For   a = [[9, 5], [6, 1]];<br/>       _b = [[3, 2], [5, 2]];<br/>bi.dotDivide(a, b)  returns [[3, 2.5], [1.2, 0.5]] |
|  <b>dotMultiply</b> | Returns the value obtained after multiplying two matrices element wise | For   a = [[9, 5], [6, 1]];<br/>       _b = [[3, 2], [5, 2]];<br/>bi.dotMultiple(a, _b)  returns [[27, 10], [30, 2]] |
|  <b>dotPow</b> | Return value after calculateing the power of x to y element wise. | For a = [[1, 2], [4, 3]];<br/>bi.dotPow(a, 2)   returns  [[1, 4], [16, 9]] |
|  <b>exp</b> | Retunr the exponentinal power of a value. | bi.exp(x)<br/>Ex: bi.exp(2) = 7.3890560989306495 |
|  <b>gcd</b> | Returns  the greatest common divisor for two or more values or arrays. | bi.gcd(a,b) = a.b/Lcm(a,b) Ex: For a= 8, b = 12 then bi.gcd(a,b) = 4 |
|  <b>hypot</b> | Returns the hypotenusa of a list with values. | bi.hypot = (p1,p2,p3..) <br/>Ex: bi.hypot (3,4) = sqrate_root ( square(3) + square(4) ) = 5 |
|  <b>lcm</b> | Returns the least common multiple for two or more values or arrays | bi.lcm(a,b)<br/>Ex: For a = 4,b = 6 then  bi.lcm(4,6) = 12 |
|  <b>log</b> | Returns the logarithm of a value (e-based). | bi.log(a)<br/>Ex: bi.log(10) = 2.3025850929 |
|  <b>log10</b> | Returns the logarithm of a value (10-based). | bi.log10(a)<br/>Ex: bi.log10(10) = 1 |
|  <b>mod</b> | Returns the remainder of an integer division of two values(Calculates the modulus) | bi.mod(a,b)<br/>Ex: For a= 17, b= 3 then bi.mod(a,b) = 2 |
|  <b>multiply</b> | Returns the value obtained after multiplying the two or more given values | bi.multiply(p1,p2,p3,....)<br/>Ex: bi.multiply(3,4) = 3*4 =12 |
|  <b>norm</b> | Returns the norm of a number, vector or matrix | bi.norm(a)<br/>Ex: norm(-3.5) = 3.5, norm([[1, 2], [3, 4]], 1) returns 6 |
| <b>nthRoot</b> | Returns the nth root calculation of given value. | bi.nthRoot(a,b)<br/>Ex: bi.nthRoot(9,2) = (3^2) = 9 |
|  <b>pow</b>| Returns the power value of the first parameter to the second parameter | bi.pow(a,b)<br/>Ex: bi.pow (5,3) = value of 5 to the power 3 = 125 |
|  <b>round</b> | Returns the rounded a value towards the nearest integer. | bi.round(A)<br/>Ex: bi.round(3.2) = 3 |
|  <b>sign</b>| Returns the sign of a value. | bi.sign(A)<br/>Ex: bi.sign (3.4) = 1 , bi.sign(-3,4)= -1 , bi.sign(0) = 0 , 1 when x > 1, -1 when x < 0, 0 when x == 0 |
|  <b>sqrt</b> | Returns the square root of given value. | bi.sqrt(x)<br/>Ex: bi.sqrt(25) = 5 |
|  <b>square</b> | Returns the square of given value. | bi.square(x)<br/>Ex: bi.square(5) = 25 |
|  <b>unaryMinus</b> | Returns the Inverse sign of a value, apply a unary minus operation. | bi.unaryMinus(x)<br/>Ex: bi.unaryMinus(3.5) = -3.5 & bi.unaryMinus(-4.2) = 4.2 |
|  <b>subtract</b> | Returns the value ontained after subtracting two given values | bi.substract(a,b)<br/>Ex: bi.subtract (4,3) = 4-3 = 1 |
|  <b>unaryPlus</b> | Returns the Inverse sign of a value, apply a unary plus operation. | bi.unaryPlus(x)<br/>Ex: bi.unaryPlus(3.44) = 3.44  |
|  <b>xgcd</b> | Returns the extended greatest common divisor for two values. | bi.xgcd(a,b) <br/>For Array type: Returns an array containing 3 integers [div, m, n] where div = gcd(a, b) and a*m + b*n = div<br/>Ex: For bi.xgcd(8,12) = [4,-1,1] |

### Matrix

|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>concat</b> | Returns the array or text after concatenating two or more texts or matrices. | bi.concat(a,b)<br/>Ex: bi.concat(“Hello” ,”  World”) = “Hello  World”<br/>For  A = [[1, 2], [5, 6]] & B = [[3, 4], [7, 8]] <br/>bi.concat(A, B) = [[1, 2, 3, 4], [5, 6, 7, 8]] |
|  <b>Cross</b> | Returns the cross product for two vectors in three dimensional space. | Ex:bi.cross(A, B) = [ a2 b3 - a3 b2, a3 b1 - a1 b3, a1 b2 - a2b1 ]  |
|  <b>det</b> | Returns the determinant of a matrix. | bi.det([[1, 2], [3, 4]]) = -2 |
|  <b>dot</b> | Returns the dot product of two vectors. | bi.dot(A, B) = a1 b1 + a2 b2 + a3 b3 + … + an bn, <br/>Ex: bi.dot([2, 4, 1], [2, 2, 3]) = 15 |
|  <b>eye</b> | Create a 2-dimensional identity matrix with size m x n or n x n. | Ex: bi.eye(3) = [[1, 0, 0], [0, 1, 0], [0, 0, 1]], <br/>       bi.eye(3, 2) = [[1, 0], [0, 1], [0, 0]] |
|  <b>filter</b> | Filter the items in an array or one dimensional matrix. | Ex: bi.filter([6, -2, -1, 4, 3], isPositive) = [6, 4, 3], <br/>       bi.Filter(["23", "foo", "100", "55", "bar"], /[0-9]+/) = ["23", "100", "55"] |
|  <b>flatten</b> | Flatten a multi dimensional matrix into a single dimensional matrix. | Ex: bi.flatten([[1,2], [3,4]]) = [1, 2, 3, 4] |
|  <b>forEach</b> | Iterate over all elements of a matrix/array, and executes the given callback function. | Ex: bi.forEach([1, 2, 3],  function(value) { console.log(value);})<br/>Return 1,2,3 |
|  <b>inv</b> | Calculate the inverse of a square matrix. | bi.inv(value)<br/>Ex: inv(x) = inv(4) = 1/4 = 0.25 |
|  <b>kron</b> | Calculates the kronecker product of 2 matrices or vectors. | bi.kron([1,1], [2,3,4]) = [ [ 2, 3, 4, 2, 3, 4 ] ] |
|  <b>map</b> | Create a new matrix or array with the results of the callback function executed on each entry of the matrix/array. | Ex: bi.map([1, 2, 3], function(value) { return value * value;})<br/>      Returns [1,4,9] |
|  <b>ones</b> | Create a matrix filled with ones. | Ex: ones(3) = [1, 1, 1], <br/>       Ones(3, 2) = [[1, 1], [1, 1], [1, 1]] |
|  <b>partitionSelect</b> | Partition-based selection of an array or 1D matrix. | Ex: function sortByLength (a, b) { <br/>       return a.length – b.length;<br/>       } <br/>bi.partitionSelect(['Langdon', 'Tom', 'Sara'], 2, sortByLength); <br/>returns 'Langdon' |
|  <b>range</b> | Create an array from a range. | bi.range(m,n)<br/>Ex: bi.range(2, 6) = [2, 3, 4, 5], <br/>      bi.range(2, -3, -1) = [2, 1, 0, -1, -2] |
|  <b>reshape</b> | Reshape a multi dimensional array to fit the specified dimensions. | bi.reshape(x, sizes)<br/>Ex: For var x = matrix([1, 2, 3, 4, 5, 6, 7, 8]);<br/>       bi.reshape(x, [2, 2, 2])  = [[[1, 2], [3, 4]], [[5, 6], [7, 8]]] |
|  <b>resize</b> | Resize a matrix | bi.resize(x, size, defaultValue) <br/>Ex: bi.resize([1, 2, 3, 4, 5], [3]) = [1,2,3], <br/>       bi.resize("hello", [8], "!") = 'hello!!!' |
|  <b>size</b> | Calculate the size of a matrix or scalar. | bi.size(x) <br/>Ex: size('hello world') = [11], <br/>For var A = [[1, 2, 3], [4, 5, 6]] then size(A) = [2, 3] |
|  <b>sort</b> | Sort the items in a matrix. | bi.sort(x, compare) <br/>Ex:  function sortByLength (a, b) {<br/>        return a.length – b.length;<br/>        } <br/>bi.sort(['Langdon', 'Tom', 'Sara'], sortByLength);<br/>Returns  ['Tom', 'Sara', 'Langdon'] |
|  <b>squeeze</b> | Squeeze a matrix, remove inner and outer singleton dimensions from a matrix. | bi.squeeze(x) <br/>Ex: For var A = zeros(3, 1); = [[0], [0], [0]] (size 3x1)<br/>       bi.squeeze(A);  returns  [0, 0, 0] (size 3) |
|  <b>subset</b> | Get or set a subset of a matrix or string. | bi.subset(value, index, replacement [, defaultValue])<br/>Ex: For var e = [];<br/>var f = subset(e, index(0, [0, 2]), [5, 6]) then  f = [[5, 6]]<br/>var g = subset(f, index(1, 1), 7, 0) then g = [[5, 6], [0, 7]] |
|  <b>trace</b> | Calculate the trace of a matrix: the sum of the elements on the main diagonal of a square matrix. | bi.trace(x)<br/>Ex: bi.trace([[1, 2], [3, 4]]) returns 5 |
|  <b>transpose</b> | Transpose a matrix. | bi.transpose(x)<br/>Ex: For  var A = [[1, 2, 3], [4, 5, 6]] then <br/>       bi.transpose(A); = [[1, 4], [2, 5], [3, 6]] |
|  <b>zeros</b> | Create a matrix filled with zeros. | Ex:var A = [[1, 2, 3], [4, 5, 6]];<br/>      bi.zeros(size(A)) returns  [[0, 0, 0], [0, 0, 0]] |

### Geometry
|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>distance</b> | Results the eucledian distance between two points in 2 and 3 dimensional spaces. | distance([x1, y1], [x2, y2]) = distance([0,0], [4,4]) = 5.6569. |

### String

|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>format</b> | Returns string format a value of any type, | bi.format(value) = 'value',<br/>Ex: bi.format(6.4)=’6.4’ & bi.format(21385, 2) = '21000' |
|  <b>print</b> | Return the results after interpolating a value into a string template | bi.print(“String $Value String”,{Value : number})<br/>Ex: bi.print('John is $age years old', {age: 8}) returns<br/> 'John mark is 8 years old' |

### Relational
|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>compare</b> | Returns -1, 1, 0 after comparing two given values<br/>Syntax: bi.compare(x,y) <br/>Returns -1 if x<y<br/>Returns 1 if x >y<br/>Returns 0 if x=y | bi.compare(6,2) = 1,<br/>bi.compare(2,6) = -1,<br/>bi.compare(6,6) = 0 |
|  <b>deepEqual</b> | Returns true / false after comparing the given values or list | bi.deepEqual(x,y)<br/>Ex: bi.deepEqual(6,8) = false , bi.deepEqual(6,6) = true<br/>For a = [2, 5, 1]  & b = [2, 7, 1] then bi.deepEqual(a, b) = false |
|  <b>equal</b> | Returns true / false after comparing the given values or list | bi.equal(x,y)<br/>Ex:  bi.equal(6,8) = false , bi.equal(6,6) = true<br/>For a = [2, 5, 1]  & b = [2, 7, 1] then bi.equal(a, b) = [true false true] |
|  <b>larger</b> | Returns true / false after validating larger value in the given values:<br/>true    -  if firstvalue is greater than second <br/>false   - if secondvalue is greater than first | bi.larger(x,y)<br/>Ex: bi.larger(2,3) = false,<br/>      bi.larger(4,3) = true |
|  <b>smaller</b> | Returns true / false after validating smaller value in the given values:<br/>true    -  if firstvalue is lesser than second <br/>false   - if secondvalue is lesser than first | bi.smaller(x,y)<br/>Ex: bi.smaller(2,3) = true,<br/>      bi.smaller(4,3) = false |
|  <b>smallerEq</b> | Returns true / false after validating smaller value in the given values: <br/>true    -  if firstvalue is  lesser or equal to the second  <br/>false   - if secondvalue is greater than first | bi.smallerEq(x,y)<br/>Ex: bi.smallerEq(2,3) = true & bi.smallerEq(3,3) = true<br/>      bi.smallerEq(4,3) = false |
|  <b>unequal</b> | Returns true / false after validating equality in the given values: <br/>true    -  if the values are not equal<br/>false   -  if the values are equal | bi.unequal(x,y)<br/>Ex: bi.unequal(2,3) = true & bi.unequal(3,2) = true<br/>      bi.unequal(3,3) = false |

### Trigonometry

|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>sin</b> | Returns the sine of a value. | bi.sin(value)<br/>Ex: bi.sin(0) = 0,bi.sin(90) = 1 |
|  <b>cos</b> | Returns the cosine of a value. | bi.cos(value)<br/>Ex: bi.cos(60) = 0.5 |
|  <b>sec</b> | Returns the secant of a value, <br/>Defined as sec(x) = 1/cos(x). | bi.sec(value)<br/>Ex: bi.sec(60) = 2 |
|  <b>csc</b> | Returns the cosecant of a value, <br/>Defined as csc(x) = 1/sin(x). | bi.csc(value)<br/>Ex: bi.csc(30) = 2 |
|  <b>tan</b> | Returns the tangent of a value.<br/>Defined as tan(x) = sin(x) / cos(x) | bi.tan(value)<br/>Ex: bi.tan(45) = 1 |
|  <b>cot</b> | Returns the cotangent of a value.<br/>Defined as cot(x) = 1 / tan(x) | bi.cot(value)<br/>Ex: bi.cot(45) = 1 |
|  <b>sinh</b> | Returns the hyperbolic sine of a value, <br/>Defined as sinh(x) = 1/2 * (exp(x) - exp(-x)). | bi.sinh(value)<br/>Ex: bi.sinh(30) = 5343237290762.231 |
|  <b>cosh</b> | Returns the hyperbolic cosine of a value, <br/>Defined as cosh(x) = 1/2 * (exp(x) + exp(-x)) | bi.cosh(value)<br/>Ex: bi.cosh(90) = 6.1020164715892E+38 |
|  <b>sech</b> | Returns the hyperbolic secant of a value, <br/>Defined as sech(x) = 1 / cosh(x). | bi.sech(value)<br/>Ex: sech(65) = 1.1800181083194122e-28 |
|  <b>csch</b> | Returns the hyperbolic cosecant of a value, <br/>Defined as csch(x) = 1 / sinh(x). | bi.csch(value)<br/>Ex: bi.csch(45) = 5.725037161098787e-20 |
|  <b>tanh</b> | Returns the hyperbolic tangent of a value, <br/>Defined as tanh(x) = (exp(2 x) - 1) / (exp(2 x) + 1). | bi.tanh(value)<br/>Ex: bi.tanh(90) = 1 |
|  <b>coth</b> | Returns the hyperbolic cotangent of a value, <br/>Defined as coth(x) = 1 / tanh(x). | bi.coth(value)<br/>Ex: bi.coth(30) = 1 |
|  <b>asin</b> | Returns the inverse sine of a value. | bi.asin(value)<br/>Ex: bi.asin(30) = 0.5 |
|  <b>acos</b> | Returns the inverse cosine of a value. | bi.acos(value)<br/>Ex: bi.acos(0.5) = 1.0471975511965979 &  bi.acos(bi.cos(1.5)) =1.5 |
|  <b>asec</b> | Returns the inverse secant of a value. | bi.asec(value)<br/>Ex: bi.asec(0.5) = 1.0471975511965979 |
|  <b>acsc</b> | Returns the inverse cosecant of a value, <br/>Defined as acsc(x) = asin(1/x). | bi.acsc(value)<br/>Ex: bi.acsc(0.5) = 0.5235987755982989 &, bi.acsc(bi.csc(1.5)) =1.5 |
|  <b>atan</b> | Returns the inverse tangent of a value. | bi.atan(value)<br/>Ex: bi.atan(0.5) = 0.4636476090008061, bi.atan(bi.tan(1.5)) = 1 |
|  <b>acot</b> | Returns the inverse cotangent of a value, <br/>Defined as acot(x) = atan(1/x). | bi.acot(value)<br/>Ex: bi.acot(0.5) = 0.4636476090008061 |
|  <b>atan2</b> | Returns the inverse tangent function with two arguments, y/x. | bi.atan2(value)<br/>Ex:  |
|  <b>asinh</b> | Returns the hyperbolic arcsine of a value, <br/>Defined as asinh(x) = ln(x + sqrt(x^2 + 1)). | bi.asinh(value)<br/>Ex: bi.asinh(0.5) = 0.48121182505960347 |
|  <b>acosh</b> | Returns the hyperbolic arccos of a value, <br/>Defined as acosh(x) = ln(sqrt(x^2 - 1) + x). | bi.acosh(value)<br/>Ex: bi.acosh(1.5) = 0.9624236501192069 |
|  <b>asech</b> | Returns the hyperbolic arcsecant of a value, <br/>Defined as asech(x) = acosh(1/x) = ln(sqrt(1/x^2 - 1) + 1/x). | bi.asech(value)<br/>Ex: bi.asech(0.5) = 1.3169578969248166 |
|  <b>acsch</b> | Returns the hyperbolic arccosecant of a value, <br/>Defined as acsch(x) = asinh(1/x) = ln(1/x + sqrt(1/x^2 + 1)). | bi.acsch(value)<br/>Ex: bi.acsch(0.5) = 1.4436354751788103 |
|  <b>atanh</b> | Returns the hyperbolic arctangent of a value, <br/>Defined as atanh(x) = ln((1 + x)/(1 - x)) / 2. | bi.atanh(value)<br/>Ex: bi.atanh(0.5) = 0.5493061443340549 |
|  <b>acoth</b> | Returns  the hyperbolic arccotangent of a value, <br/>Defined as acoth(x) = atanh(1/x) = (ln((x+1)/x) + ln(x/(x-1))) / 2. | bi.acoth(value)<br/>Ex: bi.acoth(0.5) = 0.8047189562170503 |



### Constant

|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>e, E</b> | Returns the Euler’s number, the base of the natural logarithm | 2.71828182845904 |
|  <b>i</b> | Returns Imaginary unit, defined as i*i = -1. A complex number is described as a + bi, where a is the real part, and b is the imaginary part. | sqrt(-1) |
|  <b>Infinity</b> | Returns Infinity, a number which is larger than the maximum number that can be handled by a floating point number. | Infinity |
|  <b>LN2</b> | Returns the natural logarithm of 2. | 0.6931471805599451 |
|  <b>LN10</b> | Returns the natural logarithm of 10. | 2.30258509299404 |
|  <b>LOG2E</b> | Returns the base-2 logarithm of E | 1.44269504088896 |
|  <b>LOG10E</b> | Returns the base-10 logarithm of E. | 0.43429448190325104 |
|  <b>NaN</b> | Not a number. | NaN |
|  <b>null</b> | Value null. | null |
|  <b>phi</b> | Phi is the golden ratio in math this is separately coded has unicode glyph ϕ | 1.61803398874989 |
|  <b>pi, PI</b> | Returns the value of pi which is a mathematical constant that is the ratio of a circle's circumference to its diameter. | 3.14159265358979 |
|  <b>SQRT1_2</b> | Returns the square root of 1/2. | 0.707106781186547 |
|  <b>SQRT2</b> | Returns the square root of 2. | 1.41421356237309 |
|  <b>tau</b> | Returns Tau value which is the ratio constant of a circle's circumference to radius, equal to 2 * pi. | 6.28318530717958 |
|  <b>uninitialized</b> | Constant used as default value when resizing a matrix to leave new entries uninitialized | - |
## Unit	
|Name|Description|Example|
|--|--|--|
|<b>to</b>|Returns the converted unit value of a given value|Ex: bi.unit("2 inch").to("cm") |

## Utils 	
|  Name | Description | Example |
|  :------: | :------: | :------: |
|  <b>to</b> | Returns the converted unit value of a given value | bi.unit("x unit1").to("unit2")<br/>Ex: bi.number(bi.unit("2 inch").to("cm"),"cm") = 5.08 <br/>       bi.number(bi.unit("16 bytes").to("bits"),"bits") = 128 |
|  <b>clone</b> | Clone an object. | bi.clone(x) <br/>Ex: bi.clone(“3.5”) = 3.5 |
|  <b>isInteger</b> | Returns true / false after validating the given value is integer<br/>true if the given value is integer or else false | bi.inInteger(value)<br/>Ex: bi.isInteger(2) = true, <br/>       bi.isInteger(2.5) = false |
|  <b>isNaN</b> | Returns true / false after validating the given value  whether it is NaN (not a number) | bi.isNaN(value)<br/>Ex: bi.isNaN(3) = false, <br/>      bi.isNaN(NaN) = true |
|  <b>isPositive</b> | Returns true / false after validating the given value is positive<br/>true if the given value is integer or else false | bi.isPositive(value)<br/>Ex: bi.isPositive(3) = true, <br/>      bi.isPositive(-3) = false |
|  <b>isNegative</b> | Returns true / false after validating the given value is negative<br/>true if the given value is integer or else false | bi.isNegative(value)<br/>Ex: bi.isNegative(3) = false, <br/>      bi.isNegative(-3) = true |
|  <b>isNumeric</b> | Returns true / flase after validating the given value is numeric or not | bi.isNumeric(value)<br/> Ex: bi.isNumeric(3) = true, <br/>      bi.isNumeric(“string”) = false |
|  <b>isPrime</b> | Results true / false after validating  the given value is  whether a prime number | bi.isPrime(value)<br/> Ex: bi.isPrime(3) = true, <br/>       bi.isPrime(4) = false |
|  <b>isZero</b> | Results true / false after validating  the given value is  whether it is zero | bi.isZero(value)<br/> Ex: bi.isZero(1) = false, <br/>       bi.isZero(0) = true |
|  <b>typeof<b> | Determine the type of a variable. | bi.typeof(3.5) = number, <br/>bi.typeof(math.complex('2-4i')) = complex,<br/>bi.typeof('hello world') = string |




## Arithmetic & Logical operations on Data Fields

Perform Arithmetic operation on desired fields in calculated columns.

> **For Instance:**
To calculate Average of Quantity_sum and amount 2500, derive the following expression in calculated column screen.
 ```
bi.avg( ${biplus.orders.sum_quantity}, 2500)
```

<b><i>The resultant for this expression would average values;</i></b>

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/624ab7a0166fa0c64cfdae5df07747ba80dde139/images/New_version5/TD_CC_Image6.png)

<b><font color = "Black"> Image 6</b>


## Calculate Custom Functions

It will execute a series of actions on a database record and returns a particular value.
 
 ```
/*START*/

function Fname(input_param1,input_param2,..input_ParamN)
{

Statement 1;
Statement 2;
......
Statement N;
return Outpur_value;
}
/*END*/
bi._Fname(input_param1, input_param2,..input_paramN)
```

## Access Global Parameters
 
 Global parameter is a flat file used to manipulate, control and organize the data which is not available in database and can be accessed in report.
 
 ```
 bi.in_global_keys(["ParameterColumnName"] ["DatabaseValue"],"ParameterName.Field"])
```

- <b>Parameter Column Name</b> Refer the key name from global parameter.

-  <b>Database Value</b> Refers database value.

- <b>Parameter Name Field</b> Returns the field from global parameter it is applicable in 3 different ways ;

 <b>1.</b> <b>Static value</b> Global parameters refers to a static value.

 ```
  bi.in_global_keys( ["Parameter_Column_Name "],["Reference string" ],"Global_parameter.field")
```

><b>For Instance:</b>
``` 
bi.in_global_keys( ["Station_Name"],["Station_1" ],"Calc_ONRAW.value")
```

<b>2.</b> <b>Reference value</b> Global parameters refers to reference value.

```
  bi.in_global_keys( ["Parameter_Column_Name "],["database column" ],"Global_parameter.field")
```

><b>For Instance:</b>
```
bi.in_global_keys( ["Station_Name"],[${ROOT.AUTOTEST_ORDERS.STATIONCODE_724} ],"Calc_ONRAW.value")
```

<b>3. Login Name(User Id):</b> Provide Access based on Login ID.

```
bi.in_global_keys(["ParameterColumnName","ParameterUserID"],["DatabaseField","bi._globals("#userid#")"],"ParameterName.Field"])
```

><b>For Instance:</b>
```
bi.in_global_keys( ["UserName","Login_name"],[${ROOT.EMPLOYEES.NAME_661} 
,bi._globals("#userid#")],"CalcCol_Stage2.SeizeLimit)
```

## Calculate on Raw functionality

By enabling the field <b>Calculate On Raw</b> the calculation is applied on all the rows irrespective of grouping and pivot settings, if disabled calculation applied on abstract values only.
 
<b>For Instance:</b>  Consider the below image, which represents calculated column data  with and without enabling calculate on raw by adding ' 1.5' to average value calculated earlier.

```
bi.add(${Average} ,1.5)
```
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/3fa9740bb8b424bcd962447c7ae6c297a0e7d65a/images/New_version5/TD_CC_Image7.png)

<b><font color = "Black"> Image 7</b>

## Calculate column with Pivot Offset

To calculate the quantity_sum_difference based on each month using Pivot_Offset() function, apply pivot to month field initially.
  
Enter the following expression in calculation section.
```
${biplus.orders.sum_quantity}  - bi.pivot_offset(#{biplus.orders.sum_quantity} ,0,-1)
```
![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/master/images/New_version5/TD_CC_Image8.png)
<b><font color = "Black"> Image 8</b>

The resultant obtained based on calculation applied :

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/5d41fa32b0070e4760ea200f35708a03da54e839/images/New_version5/TD_CC_Image9.png)

<b><font color = "Black"> Image 9</b>

## Local Function

Custom function is a block of code (Series of statements which intended to a particular task) with submitted inputs and derivable output. It will ease-up the process of calculations when a series of statements or actions to be repeated on set of values and its output to be derived. AcuBi supports local function which can be written inside the function body:
```
/*START*/
function fname(param1, param2, param3 ..ParamN)
{
statement 1;
statement 2;                                     * Function body *
statement 3;

Statement N;
return `;   
}
/*END*/
fname(value1, value2, value3, ..valueN)                  * Call Function *

```


<b>For Instance :</b> To calculate minimum difference value for Month <b>January</b>, write the below local function in calculated column section.

```
/*START*/
function date_avg(a){
var x=0;
if(a=="January  "){ 
{ 
x = bi.min(bi.date_diff("2019-09-01",bi.date_format(bi.current_date,"YYYY-MM-DD")),10);
}
}
return x;
}

/*END*/

 date_avg(${biplus.orders.month_whenmade} )
```

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/a85c0c174faebe147ced653e82b57e974e1c1276/images/New_version5/TD_CC_Image10.png)

<b><font color = "Black"> Image 10</b>

The resultant for above expression is shown in image below;

![enter image description here](https://raw.githubusercontent.com/sv18042016/fp1/fda5c18eb0b6d1f84a6437691facf7ade4003faa/images/New_version5/TD_CC_Image11.png)

<b><font color = "Black"> Image 11</b>
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExNzA5NTk1MzYsMTIwODU5NTYxNCwtNz
czNzQ5Njc2LC0xNzY4MzE3OTg2LDQyMDQ4ODE3Nyw0MzYyODk5
MjMsMTk0ODcyNjEyOSwtMzY2OTY3MzI5LDExNjQzMTIwNDYsNj
A5NTI3NjQxLC0xNTkzNDE3ODY2LDE0MzM5MTQ2OTksLTExNjUz
MTQzMTYsMjIxNzk4NjE5LC00OTAxNDIzNDksMzMyMzg1ODMsMT
E5MDk3NDkwMywtMTA4ODcxMjMyMiwtMzc5OTA3Mzc2LC04MDk2
OTI0ODBdfQ==
-->