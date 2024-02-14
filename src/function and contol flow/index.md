<script>
    // Make a variable called "temperature". Write some code that tells you to put on a coat if it is below 50 degrees
    let temp = 45; if(temp < 50)
     { console.log('Put on a coat'); 
}

//If it's less than 50 degrees, wear a coat.
  function tempCheck(temperature) { if (temperature < 50 && temperature >= 30) { console.log("It's chilly, don't forget your coat!"); 
}

//If it's less than 30 degrees, wear a coat and a hat.
else if (temperature < 30 && temperature >= 0) 
{ console.log("You'll need a hat as well as a coat."); 
} 

//If it's less than 0 degrees, stay inside.Otherwise, just pants and vest is fine.
else if (temperature < 0) { console.log("Just stay inside!"); 
} 
else { console.log("Just trousers and t-shirt is fine."); } 
} tempCheck(50);



function checkTemp(temp) { 
if (temp < 50 && temp >= 30) { document.write("Wear a coat"); 
}
else if (temp < 30 && temp >= 0) { document.write("Wear a coat and a hat today"); 
}
else if (temp < 0) { document.write("Just stay inside");
} 
else { document.write("There is no need to wear a coat"); } 
} checkTemp(60)

//Write a function that outputs a sentence. Then invoke that function later in your code.
function helloWorld() { console.log("Hello World!"); } helloWorld();

//Write a simple program to combine a first name and a last name inside a function. Then update the function to accept a first and last name as arguments.
function fullName(){
  let firstName = "Michael";
  let lastName = "Cudjoe";
  document.write(firstName + " "+ lastName)
}

fullName()

//Add a return statement to your 'name' function. Use that function to set the value of a variable.
function myFullName(firstName,lastName) {
  return firstName + " " + lastName;
}

document.write(myFullName("Michael", "Cudjoe"))

</script>



