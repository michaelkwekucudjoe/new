<script>
    // Make a function to return a battery status string based on the percentage
// full. More than 75 is good, less than 35 is poor, in between is moderate.
function getStatus(level) {
  if (level > 75) {
    return 'Good';
  }
  else if (level < 35) {
    return 'Poor';
  }
  else {
    return 'Moderate';
  }
}
console.log(getStatus(80));
console.log(getStatus(50));
console.log(getStatus(20));


// pseudocode response to reading list
const books =  [
  {author: "Shubhra Gupta", title: " A Life in Movies", read: true},
  {author: "Kaki Madhava Rao", title: "the Story of a Dalit Chief Secretary", read: false},
  {author: "Dante Alighieri", title: "The Divine Comedy", read: false},
  {author: "J. R. Moehringer", title: "Spare", read: false},
  {author: "Dr.Gyan Chaturvedi", title: "Pagalkhana", read: true},
  {author: "	Abhay K", title: "The Book of Bihari Literature", read: false},
  {author: "Kasturi Ray", title: "Droupadi Murmu", read: true},
  {author: "Jane Austen", title: "Pride and Prejudice", read: false},
  {author: "Honor de Balzac", title: "Le Pure Goriot", read: true},
  {author: "Abhay K", title: "Monsoon", read: false}
];

booksListed = (books, includeStatus) => {
  for (let i = 0; i < books.length; i++) {
    console.log(`${includeStatus ? books[i].read ? 'You have read ': 'You have still yet to read ' : ''}${books[i].title} by ${books[i].author}`);
  }
}

booksListed(books, true);


// pseudocode response to recipe
const recipes = [
  {
    name: "cupcakes",
    serves: 20,
    ingredients: [
      "280g self-raising flour", 
      "175g golden caster sugar", 
      "175g unsalted butter, very soft", 
      "150g pot fat-free natural yogurt", 
      "1 tsp vanilla extract", 
      "3 eggs"
    ],
    directions: 'Put ingredients in a bowl and mix them together.  Place in a cupcake tray, Bung in the oven and bake.'
  },
  {
    name: "spring rolls",
    serves: 6,
    ingredients: [
      "500g strong white flour, plus extra for dusting", 
      "7g sachet fast-action dried yeast", 
      "300ml milk", 
      "40g unsalted butter, softened at room temperature",
      "1 egg"
    ],
    directions: 'Put ingredients in a bowl and mix them together.  Roll into balls and place on a baking tray, then Bung in the oven and bake.'
  },
  {
    name: "ginger bread",
    serves: 15,
    ingredients: [
      "85g unsalted butter, softened", 
      "1 tsp ginger extract", 
      "200g icing sugar, sifted", 
      ], 
    directions: 'Put ingredients in a bowl and mix them together.  Place in bread tin and Bung in the oven and bake.'
  }
  ]

ingredientsNeed = (recipes, name) => {
  const selectedRecipe = recipes.filter((r) => r.name.toLowerCase() === name.toLowerCase())[0];

  for (let i = 0; i < selectedRecipe.ingredients.length; i++) {
    console.log(selectedRecipe.ingredients[i])
  }
}

ingredientsNeed(recipes, 'ginger bread')


// pseudocode response to fix start
fixStart = (inputWord) => {
  const firstLetter = inputWord[0].toLowerCase()
  let mutateWord = firstLetter
  
  for (let i = 1; i < inputWord.length; i++) {
    if(inputWord[i].toLowerCase() === firstLetter) {
      mutateWord += '*';
    } else {
      mutateWord += inputWord[i].toLowerCase();
    }
  };

  return mutateWord
}

console.log(fixStart('babble'));
console.log(fixStart('turtle'));

</script>

