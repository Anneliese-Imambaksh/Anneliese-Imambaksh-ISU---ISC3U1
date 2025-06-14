Menu Options
int variable “option” is initialized and set at zero
This is to set up a while loop as long as option does not equal 4, which signals the code to exit the program and output a farewell message
Switch-case for each option is established, after the program within each code is fulfilled, the code breaks and the while loop is reiterated
Adding a Service
“addAnother” is a String variable used to iterate the sequence of adding a new service at the user’s input, it is initialized as “yes” to begin the sequence
During this section of the code, the user is asked for various inputs describing their service
These inputs are added to the respective arrayLists, categories, services, and hourlyRates
This was designed so that all of the input for adding a service lined up within the arrays, for example entering category: cleaning, service name: maid service, hourlyRate: 20.00 will all be at index 0 within the arrayLists
Additionally, the services’ initial availability is set at Available here, with an arrayList that also lines up with the other ones
Browse Service Categories
To display the service categories without repeating categories, I consolidated the non-repeating categories into a second arrayList named categoriesDisplay
This arrayList is not used for anything other than to display the categories in a readable format for the user
To select the category the user is prompted to type out the category to receive input in a String format
Here we also reset the values within selections and selectionPrices which are arrayLists used to store the information of the name of the service and price of the service within the selected category
Browse Services
Using a loop the program displays the services under the category already selected and adds them into arrayLists, selections and selectionPrices
The if statement within the loop filters out services not under the intended category
serviceNum is an integer variable that increases at the end of the loop and is used as a display number along with the services in the category, their availability, and their hourlyRate
Add Services to Cart
After getting input from the user as an integer that lines up with the serviceNum, the item is added to the user’s cart
Selections and selectionPrices under the category are then added to the cartItems and cartPrices array
Within this section the cartPrices are then added to the cartTotal and the total sum is displayed
As well as the availability at the service’s index is updated to “Fully Booked”, preventing it from getting added again
Update Cart Items
Before this is selected, a smaller menu for within checking the cart is displayed, showcasing to the user the different options available, cartChoice is an integer inputted by the user to select an option
For updating cart items the user inputs 1
To update cart items first the program confirms there are items in the cart to update and that the user entered a valid option
The program then stores the service to be updated as an integer and updates the service’s availability
Prompts the user to make a new category and service option from the available services displayed
Once a valid selection is made then the updated cart is displayed and the item’s availability is updated
Remove Services from Cart
To remove an item from the cart the user inputs 2
Once a valid item is selected the cart total and items are updated and the service’s availability is updated to “Available”
Checkout
After confirming the user wants to proceed after viewing an updated cart, an invoice displaying the services and their hourly rates are displayed and the cart total
Then I added the touch of a confirmation/invoice number that is randomly generated using math methods
Additionally, after displaying the invoice the user is thanked then taken to the main menu
Exit Program
This is case 4 of the switch-case initialized at the beginning of the program, within this case a simple farewell message is displayed before terminating the program

