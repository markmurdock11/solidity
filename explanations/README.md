# Contract Explanations

## associateContractSplitter.sol

Thiss contract accepts Ether and divides it evenly amongst a group of three employees. This would be a very helpful contract for an HR department to pay lower level employees quickly, without any bearocratic red tape. 

The contract requires three payable addresses, one for each employee. You should use a constructor to avoid hardcoding addresses into your contract. From there, all that is necessary is a few functions: balance, deposit, and payable. The only weird thing you will need to account for is a potential remainder, which you should send back to HR within the deposit function. 

Here is what the code looks like in action:

![](../photos/aps_full_screen.png)


![](../photos/aps_metamask.png)


## tieredProfitSplitter

This contract accepts Ether and divides it amongst a group of employees depending on their station within the company. Depending on the tier, or level, someone is in the company, they will receive a certain percentage of the deposit. 

The code will be very similar to the associateContractSplitter.sol, except that the transfer amounts will be based on the tier of the employee. In my example, the CEO received 60%, the CTO received 25%, and Bob the employee received 15%. Any leftover wei went directly to the CEO within the deposit function. 

Here is what the code looks like in action: 


![](../photos/tieredprfit.png)