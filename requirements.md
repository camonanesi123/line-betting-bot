# Line Group Betting Bot


## summarise: Randomized generated 3 dices range in [1-6], [1-6], [1-6] according to the odds to determine whether the user wins the lottery.

## Betting rules: Before the lottery is drawn, users place bets through group commands. A user can bet in multiple ways at once


- Bet big or small:

The user enters big/100 or small/100 in the group to bet big and small If the sum of the three dice is [4-10], it means small
If the sum of the 3 dice data is [11-17], it means big. For example, if the user bet/small, if the result of the bet is small, then the user will get 2 times the reward. If the result is "big", then the user has no reward.

command: [big/100] or [big=100] means user bet 100 dollars in big.
command:[small/100] or [small=100] means user bet 100 dollars in small.

If the points of the three dice are the same, all users lose and the dealer wins

payoff: 2X

- Betting on single and double:

The user enters an odd number or an even number in the group to bet odd number, even number If the sum of the three dice is [5,7,9,11,13,15,17] , then the result is an odd number
If the sum of the 3 dice data is [4,6,8,10,12,14,16] it represents an even number.

command: [odd/100] or [odd=100] means user bet 100 dollars in odd.
command:[even/100] or [even=100] means user bet 100 dollars in even.

payoff: 2X

 If the points of the three dice are the same, all users lose and the dealer wins

- Bet on a single number:

The user enters digit/100 in the group to participate in a single-digit bet, for example, the user enters 1/100
If a dice is drawn as 1, then the user will be rewarded twice the bet amount,
If the 2 dice are 1, then the user will get 3 times the bet amount
If the 3 dice are 1, then the user will get 4 times the bet amount.

command: [1/100] or [1=100] means user bet 100 dollars on digit 1 appearance.

award:
If the number of the user's bet appears one, the user will get 2 times the reward
If the number of the user's bet appears two, the user will get 3 times the reward
If the number of the user's bet appears three, the user will get 4 times the reward

payoff: 2X, 3X, 4X


- bet on two digits

If the user enters '1/2 100' in the group, it means that the user infers that 1 and 2 will appear in the three dice of the next lottery result, if the lottery result is consistent with the user's bet. Then the user gets 6 times the reward. If there is no hit, no reward will be given.

Payoff: 6X


# Robot function:

## A robot can be in multiple groups

- Generate an ID for each customer entering the group.
Customers enter the group and generate a user ID. If the user leaves the group and then comes back in, the ID number is still used as the customer's ID.

- The administrator can recharge the customer through the command / recharge ID amount

- The robot counts the user account balance.

- The robot needs to save the results of the last 10 lottery draws

- The administrator sends a lottery command to the robot, and the robot randomly generates three pictures of different numbers of dice and sends them to the group.
 
- The user enters a command to query the betting situation of the previous round of gambling.
 
- The user enters a command to query the current round of gambling and the winning situation
 
                                   Line Robot Command
- X: Cancel the bet
- C: Check balance
- A: Check the rules of the game
- B: Stop betting and count the betting amount
- S: Enter the lottery result, the robot will display the picture (eg S123)
- Y: bank account number
- Admin Command: $ID+Amount
- N: Display past lottery records
- Play and Odds
- betting method + betting amount
- 1/100
- 1=100
- large/100
- large=100
- Small/100
- small=100
- odds/100
- odds=100
- even/100
- even=100
- 12/100
- 23=100

# rule

1 single type:
Small: The total points are 4-10 (Leopard Banker takes all)
Big: 11-17 total points (Leopard Banker takes all)
Single: The total number of points is 5.7.9.11.13.15.17 points
Double: 4.6.8.10.12.14.16 points total
Multiple: 2 times
2. Duplex
Big single, big double, small single, small double, digital size, digital single and double.
Odds: 3.3x

3 double digits
1/2 3/1
Odds: 6x
4. Single Number
Offer a 2x odds
2 out of 3 odds
3 out of 4 odds


![image](https://github.com/camonanesi123/line-betting-bot/blob/main/image/aaaa.png)
![image](https://github.com/camonanesi123/line-betting-bot/blob/main/image/ccccc.png)
![image](https://github.com/camonanesi123/line-betting-bot/blob/main/image/dddd.png)
