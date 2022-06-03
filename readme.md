# Variables

e.g:

  > *Declaring a variable along with it's type*.
    
    var card string = "Ace of Spades" 

  > *Go automatically figure out the type of varible by it's value*.   

    card := "Ace of spades"

   > *After this declaration we can re-assign the value*.
   
    card = "Five of Diamonds"
   

   > *if we try to declare and assign the variable again we will get compilation error*. 
   
    card := "Five of Diamonds"


# Functions and Return Types

> *Basic function syntax*. 

    func main() {
      card := newCard()
    }

    func newCard() string {
      return "Five of Diamonds"
    
    }
> *Key points*
 - Every function that returns a value must indicate what type value it is returning, by default void return type will be assumed.
 - Files in the same package can freely call functions defined in other files.
 

# Slices and For loops

### Array
> Fixed length list of things

### Slice
> An array that can grow or shrink. Every element in a slice must be of same type.

> Example:

    func main() {
      cards := []string {"Ace of Diamonds", newCard()}
      
      cards = append(cards, "Six of Spades") 
      
      fmt.Println(cards)
      
    }

    func newCard() string {
      return "Five of Diamonds"
    
    }
> Note: *append function doesn't modify the existing slice rather create new slice and return that new slice*. 

---
### Iteration

     func main() {
      cards := []string {"Ace of Diamonds", newCard()}
      
      cards = append(cards, "Six of Spades") 

      for i, card := range cards {
         fmt.Println(i, card)
      }
    }
    
#### Output
    0 Ace of Diamonds
    1 Five of Diamonds
    2 Six of Spades

#### New Keywords
    for
    range
    append 

# OO Approach vs GO Approach

#### Base Go types
 - string
 - integer
 - float
 - array
 - map
 


   
