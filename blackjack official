import random
import time

print("Hi, you are going to be playing Blackjack." "The goal of blackjack is to beat the dealer's hand by getting \n "
      "closest to 21 without going over.Face cards are worth 10 points. Aces are worth 11 points. "
      "\n If you go over 21 points, the dealer wins. If the dealer goes over 21, you win.  ")

for i in range(0, 1):

    print("Press ENTER to continue.")
    press_key = input()
    if press_key == any:
        continue

cards = {1: ['2 of Club, ', 2],
         2: ['3 of Club, ', 3],
         3: ['4 of Club, ', 4],
         4: ['5 of Club, ', 5],
         5: ['6 of Club, ', 6],
         6: ['7 of Club, ', 7],
         7: ['8 of Club, ', 8],
         8: ['9 of Club, ', 9],
         9: ['10 of Club, ', 10],
         10: ['Jack of Club, ', 10],
         11: ['Queen of Club, ', 10],
         12: ['King of Club, ', 10],
         13: ['Ace of Club, ', 11],
         14: ['2 of Spades, ', 2],
         15: ['3 of Spades, ', 3],
         16: ['4 of Spades, ', 4],
         17: ['5 of Spades, ', 5],
         18: ['6 of Spades, ', 6],
         19: ['7 of Spades, ', 7],
         20: ['8 of Spades, ', 8],
         21: ['9 of Spades, ', 9],
         22: ['10 of Spades, ', 10],
         23: ['Jack of Spades, ', 10],
         24: ['Queen of Spades, ', 10],
         25: ['King of Spades, ', 10],
         26: ['Ace of Spades, ', 11],
         27: ['2 of Diamond, ', 2],
         28: ['3 of Diamond, ', 3],
         29: ['4 of Diamond, ', 4],
         30: ['5 of Diamond, ', 5],
         31: ['6 of Diamond, ', 6],
         32: ['7 of Diamond, ', 7],
         33: ['8 of Diamond, ', 8],
         34: ['9 of Diamond, ', 9],
         35: ['10 of Diamond, ', 10],
         36: ['Jack of Diamond, ', 10],
         37: ['Queen of Diamond, ', 10],
         38: ['King of Diamond, ', 10],
         39: ['Ace of Diamond, ', 11],
         40: ['2 of Hearts, ', 2],
         41: ['3 of Hearts, ', 3],
         42: ['4 of Hearts, ', 4],
         43: ['5 of Hearts, ', 5],
         44: ['6 of Hearts, ', 6],
         45: ['7 of Hearts, ', 7],
         46: ['8 of Hearts, ', 8],
         47: ['9 of Hearts, ', 9],
         48: ['10 of Hearts, ', 10],
         49: ['Jack of Hearts, ', 10],
         50: ['Queen of Hearts, ', 10],
         51: ['King of Hearts, ', 10],
         52: ['Ace of Hearts, ', 11]}


deal_for_d = random.choice(list(cards.keys()))
deal_for_d1 = random.choice(list(cards.keys()))


dealer_sum = cards[deal_for_d][1]

dealer = cards[deal_for_d][0]

print("Dealer:", dealer, 'Covered Card,', " Total known sum of dealer's cards is ", dealer_sum)

del cards[deal_for_d]

deal_for_p = random.choice(list(cards.keys()))
deal_for_p1 = random.choice(list(cards.keys()))

player = cards[deal_for_p][0], cards[deal_for_p1][0]
player_sum = cards[deal_for_p][1] + cards[deal_for_p1][1]

print("You:", player, "Your total sum of cards is ", player_sum)

del cards[deal_for_p]
del cards[deal_for_p1]



print("If you would like another card, please type Hit, if not, type Stand.")
x = input()


if x == "Hit" or x == "hit":
    while x == "Hit" or x == "hit":
        deal_for_pHit = random.choice(list(cards.keys()))

        player = "".join(player)

        player += str(cards[deal_for_pHit][0])

        player_sum += cards[deal_for_pHit][1]

        print(player, "Your total sum of cards is ", player_sum)

        del cards[deal_for_pHit]

        if player_sum > 21:
            print("You've gone bust! You lose!")

            time.sleep(8)
            exit()

        print("If you would like another card, please type Hit, if not, type Stand.")
        x = input()

        if x == "Stand" or x == "stand":
            break

if x == "Stand" or x == "stand":
    while x == "Stand" or x == "stand":
        break



while True:
    if dealer_sum <= 13:
        time.sleep(3)

        deal_for_d2 = random.choice(list(cards.keys()))

        dealer += cards[deal_for_d2][0]

        dealer_sum += cards[deal_for_d2][1]

        print("\n You:", player, "Your total sum of cards is ", player_sum)
        print("The Dealer has decided to hit \n")
        time.sleep(5)
        print(" Dealer:", dealer, "Covered Card. ", "The dealer's known cards value is ", dealer_sum)

        if dealer_sum > 21:
            print("Dealer has gone bust! You win!")

    if dealer_sum >= 13:
        print("You:", player, "Your total sum of cards is ", player_sum)
        print("Dealer:", dealer, "Covered Card", "The dealer's known cards value is ", dealer_sum)

        break



time.sleep(20)

print("The game has ended.")

time.sleep(3)

print("\n The dealer will reveal his cards and it will be told who the winner will be. \n ")

time.sleep(5)

dealer += cards[deal_for_d1][0]
dealer_sum += cards[deal_for_d1][1]


print("You:", player, "Your total sum of cards is ", player_sum)
print("Dealer:", dealer, "The dealer's known cards value is ", dealer_sum)

if dealer_sum > 21:
    print("Dealer has gone bust! You win!")
    time.sleep(15)
    exit()

if dealer_sum > player_sum:
    print("Dealer wins. You lost.")
    time.sleep(15)
    exit()

if player_sum > dealer_sum:
    print("Congratulations! You WON!!!")
    time.sleep(15)
