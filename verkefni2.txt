1.
var info = {"notandi": [{"fornafn": "Daníel"}, {"eftirnafn": "Gestsson"}, {"heimasimi": "5658787"}, {"farsimi": "6983967"}]};

console.log(info.notandi[3].farsimi)
2.
console.log(family.parents.fathers[1].name)
3.
var menu = {
    name: "The Lumberjack",
    price: 9.95,
    ingredients: ["eggs", "sausage", "toast", "hashbrowns", "pancakes"]
};

console.log(menu.name + " - $" + menu.price)
console.log(menu.ingredients.toString())
4. var savingsAccount = {
    balance: 1000,
    interestRatePercent: 1,
    deposit: function addMoney(amount) {
        if (amount > 0) {
            savingsAccount.balance += amount;
        }
    },
    withdraw: function removeMoney(amount) {
        var verifyBalance = savingsAccount.balance - amount;
        if (amount > 0 && verifyBalance >= 0) {
            savingsAccount.balance -= amount;
        }
    },
    summary: function printAccountSummary(){
        console.log("Welcome!")
        console.log("Your balance is currently " + savingsAccount.balance + " and your interest rate is " + savingsAccount.interestRatePercent + "%")
    }
    // your code goes here
};
console.log(savingsAccount.summary());

5.
var donuts = [
  { type: "Jelly", cost: 1.22 },
  { type: "Chocolate", cost: 2.45 },
  { type: "Cider", cost: 1.59 },
  { type: "Boston Cream", cost: 5.99 }
];

donuts.forEach(function(element){
	console.log(element.type + " donuts cost $" + element.cost + " each");
});

6.

let pizza = {
  "size": [{"small": 500}, {"medium": 800}, {"large": 1100}],
  "toppings": [{"cheese": 140}, {"ham": 160}, {"pepperoni": 160}, {"pineapple": 140}],
  total: function totalPizza(size, topping1, topping2) {
    return size + topping1 + topping2;
  }  
};
