---
title: IT vending machine
layout: post
author: jack.morgan2
permalink: /it-vending-machine/
source-id: 1G7J6ZfexxDQfuEDXXnRJNJ3CrPU3cAyIK9PbLKOfo7Q
published: true
---
**Normal English:**

Human:

Items needed:  Vending machine

		   Money

Method:

1. Decide what you want

2. Put the Right amount of Money into machine

    1. If money doesn't work, take it out of tray and repeat from step 2 and onwards

    2. If still not working, use a different coin

    3. If still not working, tell an employee

    4. If out of stock, choose a different item and repeat step 2 and onwards

3. Reach into tray at bottom and pull out desired item

    5. If not desired item, tell an employee and then repeat all of the steps

    6. If item gets stuck or does not come out, tell an employee and then repeat all of the steps

4. Collect change from tray at bottom

    7. If not correct change, tell and employee and then repeat all steps again

Vending machine:

	Display " 5p, 10p, 20p, 50p, £1 and £2 coins accepted only"

	If Money placed into machine, check for amount and display balance

	If money is invalid, send out of machine and ask for correct amount

	If number inputted into machine, check that enough money has been put in

	If not enough money inserted, ask for correct amount.

 send electrical current to item slot

	If item out of stock, ask for a different selection

	Spin motor, releasing item

	Calculate change ( Money inserted - item cost)

	Release change

	Display "have a nice day"

**Pseudo Code:**

Machine

WHILE True

	balance← 0

	Number_of_coins_in_the_column←0

	Return_press←0

	SUBROUTINE

		A1_Check_stock()

			If A1_tray_weight ≥ 1 THEN

				A1_stock ← 1

			ENDIF

			If A1_tray_weight ≤ 1 THEN

				A1_stock ← 0

			ENDIF

	ENDSUBROUTINE

	SUBROUTINE

		A2_Check_stock()

			If A2_tray_weight ≥ 1 THEN

				A2_stock ← 1

			ENDIF

			If A2_tray_weight ≤ 1 THEN

				A2_stock ← 0

			ENDIF

	ENDSUBROUTINE

	SUBROUTINE

		A3_Check_stock()

			If A3_tray_weight ≥ 1 THEN

				A3_stock ← 1

			ENDIF

			If A3_tray_weight ≤ 1 THEN

				A3_stock ← 0

			ENDIF

	ENDSUBROUTINE

	SUBROUTINE

		Drop_down_A1()

			A1_Motor ← 1

			Wait 3 seconds

			A1_Motor ← 0

	ENDSUBROUTINE

	SUBROUTINE

		Drop_down_A2()

			A2_Motor ← 1

			Wait 3 seconds

			A2_Motor ← 0

	ENDSUBROUTINE

	SUBROUTINE

		Drop_down_A3()

			A3_Motor ← 1

			Wait 3 seconds

			A3_Motor ← 0

	ENDSUBROUTINE

			

	REPEAT

		DISPLAY " 5p, 10p, 20p, 50p, £1 and £2 coins accepted only. Everything costs £1"

		DISPLAY " We have Polos (A1), Twix (A2) and Twinkies (A3)"

	UNTIL tray weight > 1

	IF tray weight ≥  1 THEN 

		Validate_coin()

		Number_of_coins_in_the_column ← Number_of_coins_in_the_column + 1

		Balance ← Number_of_coins_in_the_column * Coin_worth

		DISPLAY balance

	ENDIF

	IF balance ≥ £1 THEN

		Display "What would you like?"

	ENDIF

	Order ← USERINPUT

IF order = A1 THEN

		A1_Check_stock()

		IF A1_Check_in_stock = 1 THEN

			Drop_down_A1()

		ENDIF

		IF A1_Check_in_stock = 0 THEN

DISPLAY "That item is out of stock, try a different item or press the return button for your money back"

ENDIF

		IF return_press = 1 THEN

			Return_money()

		ENDIF

	ENDIF

	IF order = A2 THEN

		A2_Check_stock()

		IF A2_Check_in_stock = 1 THEN

			Drop_down_A2()

		ENDIF

		IF A2_Check_in_stock = 0 THEN

DISPLAY "That item is out of stock, try a different item or press the return button for your money back"

ENDIF

		IF return_press = 1 THEN

			Return_money()

		ENDIF

	ENDIF

	IF order = A3 THEN

		A3_Check_stock()

		IF A3_Check_in_stock = 1 THEN

			Drop_down_A3()

		ENDIF

		IF A3_Check_in_stock = 0 THEN

DISPLAY "That item is out of stock, try a different item or press the return button for your money back"

ENDIF

		IF return_press = 1 THEN

			Return_money()

		ENDIF

	ENDIF

	Return_money()

	

	

	

	

	

	

	

	

	

	

	

	

	

	

	

