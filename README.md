#Solidity Assessment 

This file is all about the final project ETH PROOF: Begginer EVM Course.

##PROJECT:  Create A Project Token
In this code we will show us how to mint our first ever toke, and will also show how to burn
it afterwards

##IDE
Go ahead https://remix.ethereum.org/ a online IDE to create our Program

#EXECUTING THE PROGRAM

##MINTING PROCESS
      // mint function
    function mint (address _address, uint _value) public {
        totalSupply += _value; 
        balances[_address] += _value;

    }
}
We Createed a function with a purpose of Minting the Token thus we called it Mingting. 
We will get the address with a value of _address and a none negative number for the value
for the value of our token. 

the 'totalSupply' will show us the total supply of our token after minting the balance will shouw us the total balance in our
address minting.

##BURNING PROCESS

        if (balances[_address] >= _value){
        totalSupply -= _value; 
        balances[_address] -= _value;
        }
    }
}

We created a function with a purpose of Burning the token and we will call it Burning
We will get the address with a value of _address and a none negative number for the value of our token

then the 'totalSupply' will show us the total supply of our token after doing the burning process
the balance will show us the total balance of the token in our address after the burning process.
