Генерация пароля для ленточного накопителя HP.


Ленточный накопитель HPE Ultrium является сложным ИТ оборудование для осуществления задач резервного копирования на картриджи LTO. Возникаю ситуации, когда администратор по той или и ной причини забывает или не знает пароль доступа в меню накопителя. В таких случаях для сброса пароля необходимо было обращаться к производителю оборудования, к сожалению в текущей политической ситуации это не возможно всвязи с уходом вендора из РФ. Но есть обходное решение, это вход по мастер паролю который меняется каждый час. Пароль представляет из себя 8 цифр. Алгоритм по получению мастер пароля в приложении к текущей задаче (на англ.). Прошу разработать программный продукт, который на основании текущей даты, выдает мастер пароль.


The following is required before resetting the password:

Access to the front panel of the HP Surestore DLT library.
From the Home screen, press Main.
From Main, press Information.
From Information, press More.
From this menu, press Date and Time.
Write down the date (including year) and time.
The display shows a valid date and time
Do the following:

Press the left-most button (button 1). This button is not labeled. A warning message to call service will appear.
Press OK.
The Call Center must then calculate a special password based on the date and time, using the following formula:
(Hours * 1001) + (Days * 101) + Month + Year (all 4 digits) = subtotal
Multiply the subtotal by 123. If this multiplication results in a number greater than 99,999,999 (this should never happen), use the special password of 44122333.
Since the only valid choices are 1-4 for each digit, follow these rules:
If the digit=0 (zero), make the digit=1
If the digit=9, then make digit=1
If the digit>4, subtract 4 from the digit
If the digit does not meet any of the above, leave the digit unchanged. If the result is less than 8 digits, add leading 1s to make it eight digits in length.
NOTE: As an example, 2000 02/07 2:30 is displayed (February 7, 2000 at 2:30). Plugging in the numbers: (2 * 1001) + (7 * 101) + 2 + 2000 = 4711
4711 * 123 = 59453
Convert all digits to be between 1 and 4 = 131413
Add the leading 1s to make it eight digits long - 11131413
Enter this special code to the front panel.
Press OK. The screen will confirm that the password has been reset.
Set a new password.