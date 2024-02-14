<script>
//Create a function that is able to return a specific percentage of any number.For example you want to know what 30% of 135 is.
const number = 135
const percentage = 30
percentageCalculator = (number, percentage) => {
  return (number * percentage) / 100
}
console.log(percentageCalculator(number, percentage));
console.log(percentageCalculator(135, 30));
console.log(Number); 
const result = percentageCalculator(number, percentage);
alert(`${percentage} of ${Number} is : ${result}`)

//Customers can order 3 different types of drink and also select 3 sizes.Cola, Lemonade and  Orangeade.Small, Medium and Large.The button they press have the values “cola”,”lemon”,”orange”.Create a function that will output the message “You have ordered a {size} of {softDrinkLabel}”
      drinkOrder = (fav, size) => {
  let drinklable = '';
  const Size = ['small', 'medium', 'large']
  const flavours = ['cola', 'lemon', 'orange']
  
  if (flavours.includes(fav.toLowerCase()) &&
     sizes.includes(size.toLowerCase())) {
    switch(fav.toLowerCase()) {
         case 'lemon':
      drinkLabel = 'Lemonade';
      break;
      
    case 'cola':
      drinkLabel = 'Cola';
      break;
      
    default:
      drinkLabel = Orangeade;
      break;
    }
    return `You have ordered a ${size} ${drinkLabel}.`;
  }
  
}

console.log(drinkOrder('medium', 'cola'));
console.log(drinkOrder('medium', 'lemon'));

//We need to create a function capable of using the addition, subtraction, multiply, divider or modulus operator on 2 numbers provided.
calculator = (number1, number2, operator) => {
        switch(operator) {
          case '+':
            return number1 + number2;
          case '-':
            return number1 - number2;
          case '/':
            return number1 / number2;
          case '*':
            return number1 * number2;
          case '%':
            return number1 % number2;
        }
          
  const result = calculator(number1, number2, operator); 
       
        return (`${number1}${operator}${number2} is equal to ${result}`)
}

console.log(calculator(50,20,'-'));

</script>
 