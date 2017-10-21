# CurrencyConvert
This is a java script currency converter

/* //This is a Javascript document.

You are to create a program that can convert money from one system to another.

At the start of your program, ask the user how much money they have. Next ask them 

what currency they have and finally ask them what they want to convert it into. 

Convert the currency to the requested output and print a nice alert message with 

the value in the other currency.

Use the following currencies and conversion rates:

1 USD = 0.91 Euro
1 USD = 124.17 JP Yen
1 USD = 0.65 British Pound
1 USD = 3.51 Brazilian Real
You can use math to figure out what all of these are equal to relative to one another.

Use the following as allowed input for the currency:

'USD'
'EUR'
'GBP'
'JPY'
'BRL' 
*/

"use strict";

let rates = [

    0.65,
    1.53,
    3.51,
    0.28,
    124.17,
    0.08,
    0.91,
    1
    

   

];

let USD_GBP = rates [0];
let GBP_USD = rates [1];
let USD_BRL = rates [2];
let BRL_USD = rates [3];
let USD_JPY = rates [4];
let JPY_USD = rates [5];
let EUR_USD = rates [6];
let USD_EUR = rates [7];



let result = 0;
let amount = 0;

let amnt = (prompt("How much money do you have?"));
let cf = (prompt("What currency do you have? ( in USD, EUR, JPY, GBP, BRL."));
let ct = (prompt("What currency do you want? ( in USD, EUR, JPY, GBP, BRL."));


 converter = convertCurrencies(amnt, cf, ct);


function convertCurrencies (amount, convertFrom, convertTo) {
   

    console.log(coverter);
  
      if (convertFrom == "1 USD" && convertTo == "1 * 0.65 GBP") {
        result = amount = USD_GBP;

     }else if (convertFrom == "1 GBP" && convertTo == "1/0.65 USD") {
        result = amount = GBP_USD;
    } else if (convertFrom == "1" && convertTo == "1 * 3.51") {
        result = amount = USD_BRL;
    } else if (convertFrom == "1" && convertTo == "1/3.51") {
        result = amount = BRL_USD;
    } else if (convertFrom == "1 USD" && convertTo == "1 * 124.17") {
        result = amount = USD_JPY;
    } else if (convertFrom == "1/124.17 JPY" && convertTo == "1 USD") {
        result = amount = JPY_USD;
    }else if (convertFrom == "1/0.91 EUR" && convertTo =="1 USD") {
        result = amount = EUR_USD;
    }else if (convertFrom == "1" && convertTo == "1 * 0.91") {
        result = amount = USD_EUR;
    } else if (convertFrom === convertTo) {
        result = amount;
        console.log(amount + "" + convertFrom + "  " + result + "" + convertTo);
    } else { 
        alert("Error");
    }
    

}












 
