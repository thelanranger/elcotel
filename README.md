How to:

1) Setup PNM Plus in either a VM or physica machine. You will need a modem that is capable of contacting the payphone. (Note that I was never able to get PNM to dial the phone, only the phone to dial the PNM poller.)
2) Copy the r94 files to the PNMPLUS\DBCONFIG folder.
3) Start the Operator Console and create a new phone. Enter the dial from number (this does not really matter as we cannot control the dial from area code), the phone ID, and a Location.
4) Click the "Rates" button and choose either QUARTERS or FREEPLAY respectively and hit 'Assign to phone'.
5) Hit OK and open the PNM Polling Manager.
6) Have your phone dial the system and verify that the programming was successful. Instructions for dial to in the included PDFs.

Dial to instructions:
1) Open the Polling Manager and be certain the modem is online (call the polling manager with a phone and make sure it answers with a modem tone).
2) Reset your payphone to factory.
    2a) Go on hook for at least 5 seconds.
    2b) Hold down the reset button the main board and go off hook. Wait for the relays to fire.
    2c) Enter 122 and listen for the response "OK".
    2d) The phone should now be reset.
3) Go off hook and enter #99999999 and listen for the Voice prompt then enter 333. You should get a response of 333 ZERO or 333 and a phone number. This is the number that the payphone will dial to contact the polling manager. Dial * the number of the polling manager *. Listen for the voice prompt to confirm.
4) Enter 402 and listen for the response. Then enter * and the ID of the phone in the phone configuration * and listen for the prompt. (If your phone ID is 1234 it should respond 402 1234.)
5) Enter 961 and go on hook. Typically you may hold down the switch and use the handset to listen for the modem of the phone to dial. This can be helpful in diagnosing issues with the dialing proceedure.


IMPORTANT NOTE: This rate file is a modification of the default file! Regardless of the area code you use for your phone number the phone will always program itself with a 941 area code. (If your phone is 555-555-1212 in the operating manager, after programming, #88888888, 333 will return "3339415551212" meaning that the password has been changed from default to bypass, and the phone is now responding as the requested number, dialing from 941.) The general purpose of this file is mass program all codes for a flat rate so you can dial out from your house. Service numbers and speed dials can also be assigned to the phones but the phone will always presume it is dialing from 941 area code. 
