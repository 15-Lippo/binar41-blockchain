# binar41-blockchain
blockchain binar41
{
​ "ApplicationName": "binar41",
​ "DisplayName": "binar41!",
​ "Description": "A simple application to send request and get response",
​ "ApplicationRoles": [
​ ​ {
​ ​ ​ "Name": "Requestor",
​ ​ ​ "Description": "A person sending a request."
​ ​ },
​ ​ {
​ ​ ​ "Name": "Responder",
​ ​ ​ "Description": "A person responding to a request"
​ ​ }
​ ],
​ "Workflows": [
​ ​ {
​ ​ ​ "Name": "binar41",
​ ​ ​ "DisplayName": "Request Response",
​ ​ ​ "Description": "A simple workflow to send a request and receive a response.",
​ ​ ​ "Initiators": [ "Requestor" ],
​ ​ ​ "StartState": "Request",
​ ​ ​ "Properties": [
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "State",
​ ​ ​ ​ ​ "DisplayName": "State",
​ ​ ​ ​ ​ "Description": "Holds the state of the contract.",
​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ "Name": "state"
​ ​ ​ ​ ​ }
​ ​ ​ ​ },
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "Requestor",
​ ​ ​ ​ ​ "DisplayName": "Requestor",
​ ​ ​ ​ ​ "Description": "A person sending a request.",
​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ "Name": "Requestor"
​ ​ ​ ​ ​ }
​ ​ ​ ​ },
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "Responder",
​ ​ ​ ​ ​ "DisplayName": "Responder",
​ ​ ​ ​ ​ "Description": "A person sending a response.",
​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ "Name": "Responder"
​ ​ ​ ​ ​ }
​ ​ ​ ​ },
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "RequestMessage",
​ ​ ​ ​ ​ "DisplayName": "Request Message",
​ ​ ​ ​ ​ "Description": "A request message.",
​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ "Name": "string"
​ ​ ​ ​ ​ }
​ ​ ​ ​ },
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "ResponseMessage",
​ ​ ​ ​ ​ "DisplayName": "Response Message",
​ ​ ​ ​ ​ "Description": "A response message.",
​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ "Name": "string"
​ ​ ​ ​ ​ }
​ ​ ​ ​ }
​ ​ ​ ],
​ ​ ​ "Constructor": {
​ ​ ​ ​ "Parameters": [
​ ​ ​ ​ ​ {
​ ​ ​ ​ ​ ​ "Name": "message",
​ ​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ ​ "DisplayName": "Request Message",
​ ​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ ​ "Name": "string"
​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ }
​ ​ ​ ​ ]
​ ​ ​ },
​ ​ ​ "Functions": [
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "SendRequest",
​ ​ ​ ​ ​ "DisplayName": "Request",
​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ "Parameters": [
​ ​ ​ ​ ​ ​ {
​ ​ ​ ​ ​ ​ ​ "Name": "requestMessage",
​ ​ ​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ ​ ​ "DisplayName": "Request Message",
​ ​ ​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ ​ ​ "Name": "string"
​ ​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ ]
​ ​ ​ ​ },
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "SendResponse",
​ ​ ​ ​ ​ "DisplayName": "Response",
​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ "Parameters": [
​ ​ ​ ​ ​ ​ {
​ ​ ​ ​ ​ ​ ​ "Name": "responseMessage",
​ ​ ​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ ​ ​ "DisplayName": "Response Message",
​ ​ ​ ​ ​ ​ ​ "Type": {
​ ​ ​ ​ ​ ​ ​ ​ "Name": "string"
​ ​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ ]
​ ​ ​ ​ }
​ ​ ​ ],
​ ​ ​ "States": [
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "Request",
​ ​ ​ ​ ​ "DisplayName": "Request",
​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ "PercentComplete": 50,
​ ​ ​ ​ ​ "Value": 0,
​ ​ ​ ​ ​ "Style": "Success",
​ ​ ​ ​ ​ "Transitions": [
​ ​ ​ ​ ​ ​ {
​ ​ ​ ​ ​ ​ ​ "AllowedRoles": ["Responder"],
​ ​ ​ ​ ​ ​ ​ "AllowedInstanceRoles": [],
​ ​ ​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ ​ ​ "Function": "SendResponse",
​ ​ ​ ​ ​ ​ ​ "NextStates": [ "Respond" ],
​ ​ ​ ​ ​ ​ ​ "DisplayName": "Send Response"
​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ ]
​ ​ ​ ​ },
​ ​ ​ ​ {
​ ​ ​ ​ ​ "Name": "Respond",
​ ​ ​ ​ ​ "DisplayName": "Respond",
​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ "PercentComplete": 90,
​ ​ ​ ​ ​ "Value": 1,
​ ​ ​ ​ ​ "Style": "Success",
​ ​ ​ ​ ​ "Transitions": [
​ ​ ​ ​ ​ ​ {
​ ​ ​ ​ ​ ​ ​ "AllowedRoles": [],
​ ​ ​ ​ ​ ​ ​ "AllowedInstanceRoles": ["Requestor"],
​ ​ ​ ​ ​ ​ ​ "Description": "...",
​ ​ ​ ​ ​ ​ ​ "Function": "SendRequest",
​ ​ ​ ​ ​ ​ ​ "NextStates": [ "Request" ],
​ ​ ​ ​ ​ ​ ​ "DisplayName": "Send Request"
​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ ​ ]
​ ​ ​ ​ }
​ ​ ​ ]
​ ​ }
​ ]
}

binar41 Blockchain.sol
// constructor function
​ ​ constructor(string memory message) public
​ ​ {
​ ​ ​ ​ Requestor = msg.sender;
​ ​ ​ ​ RequestMessage = message;
​ ​ ​ ​ State = StateType.Request;
​ ​ }
contract binar41Blockchain {
pragma solidity >=0.4.25 <0.6.0;

pragma solidity >= 0.7.0 <0.8.0;

contract binar41 {
​ ​ // The keyword "public" makes variables
​ ​ // accessible from other contracts
​ ​ address public minter: qpnspxwnftc9yw84p796kwsa7328muyc9yjlunckt9;
​ ​ mapping (address => uint) public balances;

​ ​ // Events allow clients to react to specific
​ ​ // contract changes you declare
​ ​ event Sent (address from, address to, uint amount);

​ ​ // Constructor code is only run when the contract
​ ​ // is created
​ ​ constructor() public {
​ ​ ​ ​ minter = msg.sender;
​ ​ }

​ ​ // Sends an amount of newly created coins to an address
​ ​ // Can only be called by the contract creator
​ ​ function mint(address receiver, uint amount) public {
​ ​ ​ ​ require(msg.sender == minter);
​ ​ ​ ​ require(amount < 1e60);
​ ​ ​ ​ balances[receiver] += amount;
​ ​ }

​ ​ // Sends an amount of existing coins
​ ​ // from any caller to an address
​ ​ function send(address receiver, uint amount) public {
​ ​ ​ ​ require(amount <= balances[msg.sender], "Insufficient balance.");
​ ​ ​ ​ balances[msg.sender] -= amount;
​ ​ ​ ​ balances[receiver] += amount;
​ ​ ​ ​ emit Sent (msg.sender, receiver, amount);
​ ​ }
}


// SPDX-License-Identifier: GPL-3.0

pragma solidity >=0.7.0 <0.9.0;

/**
​ * @title Storage
​ * @dev Store & retrieve value in a variable
​ */
contract Storage {

​ ​ uint256 number;

​ ​ /**
​ ​ ​ * @dev Store value in variable
​ ​ ​ * @param num value to store
​ ​ ​ */
​ ​ function store(uint256 num) public {
​ ​ ​ ​ number = num;
​ ​ }

​ ​ /**
​ ​ ​ * @dev Return value
​ ​ ​ * @return value of 'number'
​ ​ ​ */
​ ​ function retrieve() public view returns (uint256){
​ ​ ​ ​ return number;
​ ​ }
}



// SPDX-License-Identifier: GPL-3.0

pragma solidity >=0.7.0 <0.9.0;

/**
​ * @title Ballot
​ * @dev Implements voting process along with vote delegation
​ */
contract Ballot {
​ ​
​ ​ struct Voter {
​ ​ ​ ​ uint weight; // weight is accumulated by delegation
​ ​ ​ ​ bool voted; ​ // if true, that person already voted
​ ​ ​ ​ address delegate; // person delegated to
​ ​ ​ ​ uint vote; ​ // index of the voted proposal
​ ​ }

​ ​ struct Proposal {
​ ​ ​ ​ // If you can limit the length to a certain number of bytes,
​ ​ ​ ​ // always use one of bytes1 to bytes32 because they are much cheaper
​ ​ ​ ​ bytes32 name; ​ // short name (up to 32 bytes)
​ ​ ​ ​ uint voteCount; // number of accumulated votes
​ ​ }

​ ​ address public binar41;

​ ​ mapping(address => Voter) public voters;

​ ​ Proposal[] public proposals;

​ ​ /**
​ ​ ​ * @dev Create a new ballot to choose one of 'proposalNames'.
​ ​ ​ * @param proposalNames names of proposals
​ ​ ​ */
​ ​ constructor(bytes32[] memory proposalNames) {
​ ​ ​ ​ chairperson = msg.sender;
​ ​ ​ ​ voters[chairperson].weight = 1;

​ ​ ​ ​ for (uint i = 0; i < proposalNames.length; i++) {
​ ​ ​ ​ ​ ​ // 'Proposal({...})' creates a temporary
​ ​ ​ ​ ​ ​ // Proposal object and 'proposals.push(...)'
​ ​ ​ ​ ​ ​ // appends it to the end of 'proposals'.
​ ​ ​ ​ ​ ​ proposals.push(Proposal({
​ ​ ​ ​ ​ ​ ​ ​ name: proposalNames[i],
​ ​ ​ ​ ​ ​ ​ ​ voteCount: 0
​ ​ ​ ​ ​ ​ }));
​ ​ ​ ​ }
​ ​ }
​ ​
​ ​ /**
​ ​ ​ * @dev Give 'voter' the right to vote on this ballot. May only be called by 'chairperson'.
​ ​ ​ * @param voter address of voter
​ ​ ​ */
​ ​ function giveRightToVote(address voter) public {
​ ​ ​ ​ require(
​ ​ ​ ​ ​ ​ msg.sender == chairperson,
​ ​ ​ ​ ​ ​ "Only chairperson can give right to vote."
​ ​ ​ ​ );
​ ​ ​ ​ require(
​ ​ ​ ​ ​ ​ !voters[voter].voted,
​ ​ ​ ​ ​ ​ "The voter already voted."
​ ​ ​ ​ );
​ ​ ​ ​ require(voters[voter].weight == 0);
​ ​ ​ ​ voters[voter].weight = 1;
​ ​ }

​ ​ /**
​ ​ ​ * @dev Delegate your vote to the voter 'to'.
​ ​ ​ * @param to address to which vote is delegated
​ ​ ​ */
​ ​ function delegate(address to) public {
​ ​ ​ ​ Voter storage sender = voters[msg.sender];
​ ​ ​ ​ require(!sender.voted, "You already voted.");
​ ​ ​ ​ require(to != msg.sender, "Self-delegation is disallowed.");

​ ​ ​ ​ while (voters[to].delegate != address(0)) {
​ ​ ​ ​ ​ ​ to = voters[to].delegate;

​ ​ ​ ​ ​ ​ // We found a loop in the delegation, not allowed.
​ ​ ​ ​ ​ ​ require(to != msg.sender, "Found loop in delegation.");
​ ​ ​ ​ }
​ ​ ​ ​ sender.voted = true;
​ ​ ​ ​ sender.delegate = to;
​ ​ ​ ​ Voter storage delegate_ = voters[to];
​ ​ ​ ​ if (delegate_.voted) {
​ ​ ​ ​ ​ ​ // If the delegate already voted,
​ ​ ​ ​ ​ ​ // directly add to the number of votes
​ ​ ​ ​ ​ ​ proposals[delegate_.vote].voteCount += sender.weight;
​ ​ ​ ​ } else {
​ ​ ​ ​ ​ ​ // If the delegate did not vote yet,
​ ​ ​ ​ ​ ​ // add to her weight.
​ ​ ​ ​ ​ ​ delegate_.weight += sender.weight;
​ ​ ​ ​ }
​ ​ }

​ ​ /**
​ ​ ​ * @dev Give your vote (including votes delegated to you) to proposal 'proposals[proposal].name'.
​ ​ ​ * @param proposal index of proposal in the proposals array
​ ​ ​ */
​ ​ function vote(uint proposal) public {
​ ​ ​ ​ Voter storage sender = voters[msg.sender];
​ ​ ​ ​ require(sender.weight != 0, "Has no right to vote");
​ ​ ​ ​ require(!sender.voted, "Already voted.");
​ ​ ​ ​ sender.voted = true;
​ ​ ​ ​ sender.vote = proposal;

​ ​ ​ ​ // If 'proposal' is out of the range of the array,
​ ​ ​ ​ // this will throw automatically and revert all
​ ​ ​ ​ // changes.
​ ​ ​ ​ proposals[proposal].voteCount += sender.weight;
​ ​ }

​ ​ /**
​ ​ ​ * @dev Computes the winning proposal taking all previous votes into account.
​ ​ ​ * @return winningProposal_ index of winning proposal in the proposals array
​ ​ ​ */
​ ​ function winningProposal() public view
​ ​ ​ ​ ​ ​ returns (uint winningProposal_)
​ ​ {
​ ​ ​ ​ uint winningVoteCount = 0;
​ ​ ​ ​ for (uint p = 0; p < proposals.length; p++) {
​ ​ ​ ​ ​ ​ if (proposals[p].voteCount > winningVoteCount) {
​ ​ ​ ​ ​ ​ ​ ​ winningVoteCount = proposals[p].voteCount;
​ ​ ​ ​ ​ ​ ​ ​ winningProposal_ = p;
​ ​ ​ ​ ​ ​ }
​ ​ ​ ​ }
​ ​ }

​ ​ /**
​ ​ ​ * @dev Calls winningProposal() function to get the index of the winner contained in the proposals array and then
​ ​ ​ * @return winnerName_ the name of the winner
​ ​ ​ */
​ ​ function winnerName() public view
​ ​ ​ ​ ​ ​ returns (bytes32 winnerName_)
​ ​ {
​ ​ ​ ​ winnerName_ = proposals[winningProposal()].name;
​ ​ }
}


contract binar41Blockchain {
