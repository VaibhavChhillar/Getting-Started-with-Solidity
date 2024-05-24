[CREATING A TOKEN.md.docx](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/files/15429292/CREATING.A.TOKEN.md.docx)

**CREATING A TOKEN!**
Creating our own token 
**Description**
1.	Introduction to Data Types
2.	Mapping in Solidity
3.	Functions Demonstration
   
**Getting Started**
**Installing**
•	You can use the online Ethereum IDE 

**Executing program**
•	Go to Ethereum IDE(https://remix.ethereum.org/)  
•	Create a new file and write your code 
•	// SPDX-License-Identifier: MIT
•	pragma solidity 0.8.18;

•	contract MyToken {
•	
•	    // public variables here
•	    string public tokenName = "META";
•	    string public tokenAbbrv = "MTA";
•	    uint public totalSupply = 0;
•	
•	    // mapping variable here
•	    mapping(address => uint) public balances;
•	
•	    // mint function
•	    function mint (address _address, uint _value) public {
•	        totalSupply += _value;
•	        balances[_address] += _value;
•	    }
•	        
•	    // burn function
•	    function burn (address _address, uint _value) public {
•	        if (balances[_address] >= _value) {
•	         totalSupply -= _value;
•	            balances[_address] -= _value;
•	        }
•	    }
•	        
•	}
•	

•	Then complie the code using solidity compiler of IDE                                         Remember the auto compiler option should be enabled
 
•	Then go to Deploy and Run transactions
1.	Click on deploy
 
Something like this will come in the terminal
2.	Copy account and paste in the mint function address parameter and pass 1000 as value in the value parameter
3.	Then check the total supply
 
4.	Now paste the same address in the burn function and pass let say value 500 in the value parameter
5.	Then again check the total supply

 
**Help**
For any issue with the code take help of  debug option.

**Authors**
Vaibhav chhillar 
vaicozchhillar@gmail.com                                                                                                     
8053626353 

**License**
This project is licensed under the MIT License - see the LICENSE.md file for details


![image](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/assets/131567808/cffe8b9a-98b1-4dac-ab42-05edc3bd94d0)

![image](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/assets/131567808/2957b875-5f42-4a30-817e-5447c175a130)
![image](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/assets/131567808/d1e0a3e5-8049-48b8-9065-c3326e71fbc6)
![image](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/assets/131567808/53a06211-4a32-4f04-a869-be5e7be2354d)
![image](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/assets/131567808/3f84ecc7-c412-4b21-9cf7-33e9783d57b9)
![image](https://github.com/VaibhavChhillar/Getting-Started-with-Solidity/assets/131567808/8afc21c3-569f-4796-be65-0188576baa55)


