# 6. Conditional Statements

## Theory
Conditional statements help you make decisions in your code. They let your program choose what to do based on different conditions.
- **if:** Runs a block of code if a condition is true.
- **else if:** Checks another condition if the first one is false.
- **else:** Runs if none of the above conditions are true.
- **switch:** Checks one value against many possible cases.

---

## Practical Examples

### 1. if, else if, else
```js
let marks = 75;

if (marks >= 90) {
  console.log('Grade: A');
} else if (marks >= 75) {
  console.log('Grade: B');
} else if (marks >= 50) {
  console.log('Grade: C');
} else {
  console.log('Grade: D');
}
```

### 2. switch statement
```js
let day = 3;
let dayName;

switch (day) {
  case 1:
    dayName = 'Monday';
    break;
  case 2:
    dayName = 'Tuesday';
    break;
  case 3:
    dayName = 'Wednesday';
    break;
  case 4:
    dayName = 'Thursday';
    break;
  default:
    dayName = 'Other day';
}
console.log(dayName); // 'Wednesday'
```

---

## Practice Questions
1. Write a program to check if a number is positive, negative, or zero using if-else.
2. Use if-else to print "Even" if a number is even, otherwise print "Odd".
3. Write a program using switch to print the name of the day (1 for Monday, 2 for Tuesday, etc.).
4. Modify the grade example to add an "F" grade for marks below 35.
5. Try changing the value of `day` in the switch example and see the output.

---

**Tip:** Conditional statements help your code make smart decisions. Try changing the values and see how the output changes! 