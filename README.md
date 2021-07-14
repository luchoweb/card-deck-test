
# Card Deck

Because we are not always working from a blank slate, it's important for developers to be able to read preexisting code and figure out how to use it. This challenge designed to test your ability to manipulate the DOM using a preexisting class, based on parameters passed in through the url. When you load index.html, you'll see a deck of cards face down. Your challenge is to draw cards from that deck determined by parmeters passed in via the URL querystring.


## The Challenge

1. Accept parameters through the URL querystring.
2. Draw the cards that match those parameters.
3. Take a look at the existing class CardDeck, and determine how to use it to complete the test.
  

## Requirements

- You must complete the challenge within 4 hours of receiving this link.
- You may not use 3rd-party libraries.
- You may modify the class CardDeck if you like, but the task can be completed without modifying the class at all.
- The code should work in the latest version of Chrome.
  

### URL Parameters
Use the following URL parameters to determine which cards should be drawn.  You should be able to filter by more than one parameter at a time, and non-specified parameters eg: (?foo=bar) should not draw any cards.

#### cards

'cards' should accept one or more card id and draw all cards that match the requested id(s), eg: 

`index.html?cards=s-3` should draw the 3 of spades

`index.html?cards=s-3+c-9+h-A` should draw the 3 of spades, 9 of clubs, and Ace of hearts.

#### suits

'suits' should accept one or more suit name, and draw all cards that match the requested suit(s) eg:

 `index.html?suits=spades` should draw all the spades.

 `index.html?suits=spades+hearts` should draw all the spades, and all the hearts.
 
#### ranks

'ranks' should accept one or more rank value, and draw all cards that match the requested rank(s) eg:

 `index.html?ranks=3` should draw all the 3s

 `index.html?ranks=3+5+13` should draw all the 3s, 5s, and Kings

#### limit

'limit' should limit the number of cards drawn eg:

 `index.html?suits=spades&limit=4` should draw any 4 spades.

 `index.html?suits=clubs+hearts&ranks=2+6+10&limit=4` should draw any 4 of the following cards: 
 
 - 2 of clubs
 - 2 of hearts
 - 6 of clubs
 - 6 of hearts
 - 10 of clubs
 - 10 of hearts

#### BONUS: sorted

If you're still thirsty for more:
'sorted' should sort the drawn cards: grouped by suit and ordered by rank.  Ordering may be either asc or desc.
  

## Instructions

- Fork this repo to a private repo in your own GitHub account.
- Complete the challenge.
- Push your solution to your private repo.
- Share your repo with @thisanimus and @robmomary.