// SPDX-License-Identifier: MIT
pragma solidity >=0.6.12 <0.9.0;

contract Payment { 
    uint public balance; 
    uint public constant MAX_UINT = 10000; 

    function deposit(uint _amount) public { 

        require(_amount >1, "invalid amount"); 

        balance += _amount; 

    }

    function withdraw(uint _amount) public { 

        require(balance >= _amount, "Insufficient balance"); 

        balance -= _amount; 
       
        assert(_amount <= MAX_UINT); 

      
        if (balance > _amount) {
            revert("The amount withdrawal exceeds to the balance"); 
        }
    }
}
