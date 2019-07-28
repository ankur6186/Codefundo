# SECURED AND TRANSPARENT E-VOTING SYSTEM

Main Objective :
* To avoid duplicate and fake votes
* To avoid hacking/altering of Votes
* To count the votes casted for a candidate very accurately.
* To prevent illegal votes from different constituency by the same Individual.
* To attain a higher level of transparency by letting the person know for whom he/she has voted.

We  will use blockchain technology to achieve these goals.We are using consensus mechanism to achieve the required agreement on a single state of the network.

We will create one primary block chain and various unique block chains for all the contesting candidates.Primary block chain has blocks which will store the unique serial number given in the Voter ID card and private key which will be provided to the user at the time of creation of voter ID.This private key is unique to all the users.The users who have already created their voter ID can also generate their private key by contacting their respective BLO officers.Other block chains for all the Contestants will be having blocks having details of the candidates who have casted votes in their favour.By this way we can know the number of people voted for the particular candidate.

We will also create a MySQL database in which index of the MySQL table is private key generated earlier and corresponding to that his/her chosing candidate is stored.If the index is repeated(it means that vote belonging to that private key is already casted)then we will ignore this vote and will not change anything in MySQL table.By this way we can know the vote of all the private keys(users).To find the number of votes for particular candidate subtract the fake votes from length of block chain of that particular candidate.Number of minors in the blockchain are dependent on the population of that particular location.

We will create a web page for both the voter and the Candidate. The page for the Voter will show for whom he/she has voted using his unique serial number and private key, and also the page for Candidate will show the total number of votes he/she has got but he will not get to know the ID of the voters who have voted for him/her.

Technology Used:
* Azure Blockchain
* MySQL
* HTML
* CSS
* JavaScript
