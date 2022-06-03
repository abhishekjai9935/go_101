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



   
