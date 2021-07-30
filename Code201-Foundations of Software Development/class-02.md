# Inline & Block Tages
In HTML we have two type of tages ,in the picture below the different between them and some examples :

![tages](https://images.slideplayer.com/12/3384039/slides/slide_2.jpg) 
# CSS 

## Three Ways to Insert CSS

There are three ways of inserting a style sheet:

- External CSS
- Internal CSS
- Inline CSS

[Examples](https://www.w3schools.com/css/css_howto.asp)


## Rule syntax:

    style-rule ::=
    selectors-list {
      properties-list
     }
**Example** : 

      strong {
     color: red;
     }

For more Info. click [Here](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#basic_rule_syntax)

## Color in CSS
- Using the name of the color 
- using the HEX value for the color 
- Using RGB 

**Example** :

     body {
     color: red;
      }

    h1 {
    color: #00ff00;
     }

    p.ex {
    color: rgb(0,0,255);
     }

# 
![role](https://i.pinimg.com/originals/bc/97/96/bc97965579512f8a6d2303934f599c65.png)
--



## Here is three oparators in JS

### Arithmetic operators
| Operator	                       | Description |
| -----------                          | ----------- |	
|Remainder (%)	Binary operator.       |Returns the integer remainder of dividing the two operands.|	
|Increment (++)	Unary operator.        |Adds one to its operand. If used as a prefix operator (++x),returns the value of its operand after adding one; if used as a postfix operator (x++),returns the value of its operand before adding one.|	
|Decrement (--)	Unary operator.        |Subtracts one from its operand. The return value is analogous to that for the increment operator.|	
|Unary negation (-)Unary operator.     |Returns the negation of its operand.|	
|Unary plus (+)	Unary operator.        |Attempts to convert the operand to a number, if it is not already.|	
|Exponentiation operator (**)	       |Calculates the base to the exponent power, that is, base^exponent |	


### Assignment operators

| Operator	                | Description |
| -----------               | ----------- |
|Assignment	                |x = y	      | 
|Addition assignment	      |x += y	      |
|Subtraction assignment	    |x -= y	      |
|Multiplication assignment	|x *= y	      |
|Division assignment	      |x /= y	      |
|Remainder assignment	      |x %= y	      |



### Comparison operators

| Operator	                | Description |
| -----------                   | ----------- |
| Equal (==)	                |Returns true if the operands are equal.|
|Not equal (!=)  	        |Returns true if the operands are not equal.|
|Strict equal (===)	        |Returns true if the operands are equal and of the same type. See also Object.is and sameness in JS.|	
|Strict not equal (!==)	        |Returns true if the operands are of the same type but not equal, or are of different type.|	
|Greater than (>)	        |Returns true if the left operand is greater than the right operand.|	
|Greater than or equal (>=)	|Returns true if the left operand is greater than or equal to the right operand.|	
|Less than (<)	                |Returns true if the left operand is less than the right operand.|
|Less than or equal (<=)	| Returns true if the left operand is less than or equal to the right operand.|



## Decisions and Loops in JS
+ [If conditional](https://developer.mozilla.org/en-US/docs/Glossary/Conditional)

** Example (inline if ) : **

     var c = ((a < b) ? 'minor' : 'major');

** Example (if else ) : **
 
      if (field==empty) {
      Do something ;
       } else {
       Do something ;
       }

** Example ( else if) : **

![if else](https://miro.medium.com/max/1968/1*uENzVnU4d_rXpuoe9q1jsw.png)