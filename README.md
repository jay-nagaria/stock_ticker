# Read ME



Stock ticker application that can provide realtime daily stock data, from Alpha Vantage servers and for range of companies and also helps you make informed decisions by providing historic data in an easy to read visual graphs.

**Programming tools used:**<br />
Program is build purely using java and android libraries.

**Tools needed to run the program**<br />
Program needs java jdk installed and any ide with android emulator support (e.g Android Studio, Ecclipse, VSCode and many more)

**Project files and their descriptions**<br />

**MainActivity**<br />
- Splash screen displaying app logo.<br />

**HomeActivity**<br />
-	Next page contains Card View inside a ListView, displaying companies name and its stock name. <br />
-	On clicking a particular card, it will take you to next page based on company stock name<br />

**TickerActivity**<br />
-	Fetches data for a particular company based on provided stock name form previous page<br />
-	Fetch data from Alpha Vantage servers by providing “stock name” in URL.<br />
- ***Note: You have to provide your Alpha Vantage key in URL ( currenty key is set to null )***
-	Display loading screen with company logo (named by stock name in drawable folder, in real world can grab from URL) while the data is being fetched.<br />
-	Page displays company name stock name, previous day’s high, low, volume, open and close.<br />
-	Button provided to view historic data, onClick go to history page.<br />

**HistoryActivity**<br />
-	Displays graph of all past 100 days stock fluctuations.<br />
-	Below that listView with historic data details namely, date, day closing, volume and percent change in stock value from last day.<br />
-	If percent change is positive, display the value in green else in red.<br />
