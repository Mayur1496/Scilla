# Simple Contract in SCILLA
 - Contract can be used to send and recieve messages across the members registered on the ledger
 - Only admin is allowed to register members
 - Only membres are allowed to send and recieve messages
 - The cost of sending message is 10 Units
 - One who recieves message gets 10 Units
 - File messageContractAnalysis.json contains the CashFlow Analysis, warnings, gas consumption
 
 # Installing SCILLA
 The source code of SCILLA and its installation instructions can be found [here](https://github.com/Zilliqa/scilla)
 
 # Running Analysis
 After installing SCILLA
 run the following to get the analysis report in json format
 `scilla-checker -gaslimit 1000 -libdir ../scilla-v0.7.0/src/stdlib/ -cf  MessageContract.scilla | cat > messageContractAnalysis.json `
 
 - Analysis shows the cash-flow tags i.e. which variables are assosiated with money
 - Also the gas consumption to be 650 QA (smaller unit of ZIL which is Ziliqa's crypto currency)
 - More details on gas consumption calculations were found [here](https://scilla.readthedocs.io/en/latest/scilla-in-depth.html#gas-consumption-in-scilla)