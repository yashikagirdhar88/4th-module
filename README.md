# Degen-Token(ERC20)- Unlocking the future of Gaming
So, in this project we have imported openzeppelin library “ERC20”token.
Now we have wrote a contract “DegenToken” that inherits from “ERC20” contract and we declare a public variable owner in it.
 Then we have a constructor that initializes the “ERC20” token name as “Degen” and its symbol as “DGN” and we have assigned msg.sender as owner.
Now we have modifier here it restricts certain functions, allowing access to owner only , it has a require statement which checks if the caller is the owner and reverts a message provided if not.
After this we have a mint function which allow owner to mint tokens and assign them to specified account.
Next we have transfer function, having two parameters (recipient and amount), we override this function and it will return a bool value and and if the transfer of amount occur it will return “true” as value.
Next is redeem function, which allows user to redeem their tokens by effectively burning them using  _burn function.
Then we have the burn function which will destroy the specified tokens from the sender’s account by specified “amount” when we will call  _burn function. 
Next is the balanceof function having which is a view function only having one parameter that is “amount” and we override this function and function will return an unsigned integer value and this will return the balance amount . 
