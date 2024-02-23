# scanWM6.5
Windows Mobile 6.5 (2009) app for scanner-phone Zebra  MC67

# Development requirements:
Visual Studio 2008 (Professional Edition);
Microsoft Windows Mobile DTK 6.5;
For debuging:
Microsoft Windows Mobile SDK 6.0 - 6.5 prof. with emulators.
Links for download DTK/SDK:
https://archive.org/details/WMSDK

P.S:
For full operation of the emulator, with the connection to the Internet, an old OS Windows XP  - is required. I worked on windows 10-11, and Windows Mobile Center did not launch.
More details:
https://www.youtube.com/watch?v=NHEVGZBHON8
(All DTK/SDK in video, are in the link above).

To work on the MC67 device, the following programs were installed: Fusion Wireless manager for Internet connection, and DataWedge demo - for reading barcode.
Therefore, the program does not have modules for operating the scanner itself, the algorithm for launching the program is as follows:
1) We turn ON Wi-Fi, on the device through the Fusion wireless network profile;
2) Then launch DataWedge demo, to operate the laser scanner;
3) And only then our application.
NOTE:  all these applications were pre-installed. If you do not have them, you need to contact the manufacturer of the scanner.

The work of the scanner in the application itself is to place the cursor on the input field and press a special key on the device to read and insert the decrypted barcode.

I would also like to say "Thanks" to all those authors of questions on StackOverFlow who attached their http request code. This helped me a lot, and I hope this code will also help you in developing for WinCE.

#Описание:
Данная программа предназначена для ОС Windows Mobile 6.5, для устройств ТСД (Терминал Сбора Данных) имеющий 2D позиционированный лазерный сканер, способный считать QR-код.
Программа представляет собой простой интерфейс с примерным описанием логики работы сканера, например при использовании на складе для формирования отпускной накладной. Считывая коды товаров можно их передать в CRM систему, 1С или другую программу учета.

Чтобы открыть программу требуется довольно старый набор программ который уже сложно скачать с интернета, а именно: 
Visual Studio 2008 (Professional Edition);
Microsoft Windows Mobile DTK 6.5;
Для отладки:
Microsoft Windows Mobile SDK 6.0 - 6.5 prof. with emulators.
Ссылка для скачивания DTK/SDK:
https://archive.org/details/WMSDK

Используемый стек: C# .NET compact framework 3.5;