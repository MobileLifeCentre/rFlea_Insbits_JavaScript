rFlea_Insbits_JavaScript
========================
JavaScript library to work with rFlea Webapp and connect it to Insbits Server (www.insbits.com:1880).

The Example will create a rFlea object in the Insbits server with your ID. It contains 6 outputs and 1 input. If you program your rFlea with the example "rFlea_Android_TxRx" the 6 outputs correspond to Analog pins A4 and A5, and digital pins 3,10,11,12. The input corrsponds to the LED (pin 13). If the LED input receives a value 0, the onboards LED will switch off, if diferent form 0, it will switch on.

This is a plain example, minimal, on how to set up your webapp and get the messages from the rFlea Arduino boards. In the rflea.js you will set up first the conections and then add code if needed. The steps to set up your plain exmaple are as follow:

1. From the header of the rflea.js file set up the following parameters:

- The ID or unique MAC from your rFlea (check out rFlea_Arduino repository to learn how to get your rFlea number).
- The frequency that your packages will be received. This number should be power of 2 (1,2,4,8,16,32,64) being 64 the maximum. And it should be at least as big, as the one you set up in your rFlea Arduino board.

2. Copy the two files from the repository and put them in your webserver. In case you don't have one, you can use your dropbox public folder for that. Create a folder in your public folder and copy/paste the two files. Right click in rFlea.html and selsct "Copy Public Link". Add this adress to your rFlea Webapp.

Once the code is ready, you can get the data in you html file or, if needed add your own code in the area designed for that in the rflea.js file.
