=== Stock Quotes List ===
Contributors: stockdio  
Tags: stocks, ticker, quote, finance, quotes, stock, financial, index, indices, market, currencies, commodities, forex, list
License: See www.stockdio.com/wordpress for details.
Requires at least: 3.1
Tested up to: 6.6
Stable tag: 2.9.16
WordPress plugin and widget for displaying a list of stock market prices and their variations.

== Description ==

Stockdio's Stock Quotes List contains a plugin and a widget that provide the means to display a list of stock prices, market indices, currencies and commodities with their variations. Over 65 different stock exchanges and a large number of market indices, currencies and commodities are supported. Optionally, an interactive price chart can be included with the list.

If you're using the standard Gutenberg editor, the easiest way to include this plugin on your page is using the Stock Quotes List block, which is included in the Stockdio Financial Visualizations category.

If you're using a different editor o prefer to use the shortcode, below is a sample to help you start. Please be aware that most of the parameters listed below are optional, and are also available through the plugin's settings page. Any parameter you include in the shortcode will overwrite the parameter used in the settings page.

`[stock-quotes-list symbols="AAPL;MSFT;GOOG;HPQ;^SPX;^DJI;LSE:BAG" stockExchange="NYSENasdaq" width="100%" height="380" motif="financial" palette="financial-light"]`

This plugin is part of the Stockdio Financial Widgets, which also includes the following plugins and widgets:

* [Stockdio Historical Chart](https://wordpress.org/plugins/stockdio-historical-chart/)
* [Stock Market Overview](https://wordpress.org/plugins/stock-market-overview/)
* [Stock Market News](https://wordpress.org/plugins/stock-market-news/)
* [Stock Market Ticker](https://wordpress.org/plugins/stock-market-ticker/)
* [Economic & Market News](https://wordpress.org/plugins/economic-market-news/)

The following parameters are supported:

**stockExchange**: The exchange market the symbols belong to (optional). If not specified, NYSE/NASDAQ will be used by default. For a list of available exchanges please visit www.stockdio.com/exchanges.

**symbols**: A list of companies stock symbols, market index tickers, currency pairs or commodities ticker, separated by semi-colon (;) (e.g. **AAPL;MSFT;GOOG;HPQ;^SPX;^DJI;LSE:BAG**). Please review the FAQ section for additional details on how to includes indices, currencies and commodities, as well as how to specify custom names, combine data from different exchanges, etc.

**width**: Width of the list in either px or % (default: 100%).

**height**: Height of the list in pixels (default: 320px). If not specified, the list height will be calculated automatically.

**title**: Allows to specify a title for the list, e.g. Watch List (optional).

**intraday**: If enabled (true), auto refresh intraday delayed data will be used if available for the exchange. For a list of exchanges with intraday data available, please visit http://www.stockdio.com/exchanges.

**includeChart**: Allows to include an interactive chart along with the list (optional).

**chartHeight**: Height of the chart in pixels (default: 320px).

**includeLogo**: Allows to include/exclude a column with the stock logo or index country flag, if available. Use includeLogo=false to hide the logo (optional).

**logoMaxHeight**: Specify the maximum height allowed for the logo. The height may be smaller than the maximum, depending on the logo width, as it maintains the logo's aspect ratio (optional).

**logoMaxWidth**: Specify the maximum width allowed for the logo. The width may be smaller than the maximum, depending on the logo height, as it maintains the logo's aspect ratio (optional).

**includeSymbol**: Allows to include/exclude a column with the stock symbol. Use includeSymbol=false to hide the symbol (optional).

**includeCompany**: Allows to include/exclude a column with the company name. Use includeCompany=false to hide the company name (optional).

**includePrice**: Allows to include/exclude a column with the latest stock price. Use includePrice=false to hide the stock price (optional).

**includeChange**: Allows to include/exclude a column with the stock price change. Use includeChange=false to hide the price change (optional).

**includePercentChange**: Allows to include/exclude a column with the stock price percentual change. Use includePercentChange=false to hide the price percent change (optional).

**includeTrend**: Allows to include/exclude a column with the stock price trend icon (up/down/neutral). Use includeTrend=false to hide the trend icon (optional).

**includeVolume**: Allows to include/exclude a column with the latest volume. By default, volume is not visible. Use includeVolume=true to show it (optional).

**showHeader**: Allows to display the list header. Use showHeader=false to hide it (optional).

**showCurrency**: Allows to display the currency symbol next to the price, depending on the culture settings.

**allowSort**: If enabled (true), it allows the end user to sort the data by any of the fields, by clicking on the header, if this is visible.

**culture**: Allows to specify a combination of language and country settings, used to display texts and to format numbers and dates, e.g. Spanish-Spain (optional). For a list of available culture combinations please visit http://www.stockdio.com/cultures.

**motif**: Design used to display the visualization with specific aesthetics, including borders and styles, among other elements (optional). For a list of available motifs please visit www.stockdio.com/motifs.

**palette**: Includes a set of consistent colors used for the visualization (optional). For a list of available palettes please visit www.stockdio.com/palettes.

**font**: Allows to specify the font that will be used to render the chart. Multiple fonts may be specified separated by comma, e.g. Lato,Helvetica,Arial (optional).

**displayPrices**: Allows to specify how to display the prices on the chart (if enabled), using one of the following options (default: Line):

* Line
* Candlestick
* Area
* OHLC
* HLC

**allowPeriodChange**: If enabled (true), it provides a UI to allow the end user to select the period for the data to be displayed in the chart. This UI is enabled by default.

**days**: Allows to specify the number of days for the period to display in the chart (if enabled). If not specified, its default value is 365 days.

**loadDataWhenVisible**: Allows to fetch the data and display the visualization only when it becomes visible on the page, in order to avoid using calls (requests) when they are not needed. This is particularly useful when the visualization is not visible on the page by default, but it becomes visible as result of a user interaction (e.g. clicking on an element, etc.). It is also useful when using the same visualization multiple times on a page for different devices (e.g. using one instance of the plugin for mobile and another one for desktop). We recommend not using this by default but only on scenarios as those described above, as it may provide the end user with a small delay to display the visualization (optional).

== Installation ==

1. Upload the `StockdioPlugin` folder to your `/wp-content/plugins/` directory.

2. Activate the "Stock Quotes List" plugin in your WordPress administration interface.

3. If you want to change the preset defaults, go to the Stock Quotes List settings page.

4. If you're using the standard Gutenberg editor, add a Stock Quotes List block from the Stockdio Financial Visualizations category and configure it using the settings sidebar.

5. If you prefer to use the shortcode, insert the `[stock-quotes-list]` shortcode into your post content, customizing it with the appropriate parameters. You also have the option to use the Stock Quotes List widget included when you install the plugin.

6. For ease of use, a Stockdio icon is available in the toolbar of the HTML editor for certain versions of WordPress (see screenshots for details).

== Frequently Asked Questions ==

= How do I integrate the Stockdio Widgets List in my page? =

There are three options to integrate it: a. Using the Stock Quotes List block, b. Using the short code, or c. Through the use of the widget in your sidebars.

= How do I know if the Stock Exchange I need is supported by Stockdio? =

Stockdio supports over 65 different world exchanges. For a list of all exchanges currently supported, please visit [www.stockdio.com/exchanges](http://www.stockdio.com/exchanges). If the stock exchange you're looking for is not in the list, please contact us to info@stockdio.com. Once you have found in the list the stock exchange you need, you must pass the corresponding Exchange Symbol using the stockExchange parameter.

= How do I specify the symbols to display? =

You can specify as many symbols as you want, from the selected exchange, separated by semi-colon (;). If any of the symbols you want to display does not show up, you can go to [http://finance.stockdio.com](http://finance.stockdio.com) to verify if the symbol is currently available in Stockdio. If the symbol you require is missing, please contact us at info@stockdio.com.

= Can I combine more than one stock exchange on the same list? =

Yes. The exchange you define in the stockExchange parameter will be the default stock exchange to be used. However, if you want to include symbols from a different exchange, you must prefix the symbol with the exchange code and a colon (:). For example, if you want to include two symbols from NYSE/Nasdaq but additionally include one symbol from London Stock Exchange, you would specify stockExchange="NYSENasdaq", and symbols="AAPL;MSFT;LSE:BAG". This will also allow you to combine stocks with commodities and currencies in the same quote list.

= Can I include one or more market indices in the quotes list? =

Yes, you can include indices in the symbols parameter, using the ^ prefix. For example, use ^SPX for S&P 500 or ^DJI for the Dow Jones. For a complete list of indices currently supported, please visit [www.stockdio.com/indices](http://www.stockdio.com/indices)

= Can I create a Commodities list? =

Yes. You must use **COMMODITIES** as the stockExchange and then specify one or more commodities in the symbols parameter. For example, use GC;SI;CL for Gold, Silver and Crude Oil. For a complete list of commodities currently supported by Stockdio, please visit [www.stockdio.com/commodities](http://www.stockdio.com/commodities)

= Can I create a Currencies list? =

Yes. You must use **FOREX** as the stockExchange and then specify one or more currency pairs in the symbols parameter. For example, use EUR/USD, USD/JPY, GBP/USD for Euro vs. USD, USD vs. Japanese Yen and British Pound vs. USD. For a complete list of currencies currently supported by Stockdio, please visit [www.stockdio.com/currencies](http://www.stockdio.com/currencies)

= I would like to specify a custom name for a given symbol. Can I do that? =

Yes, we understand there are several scenarios in which you may want to display your own name, such as if you would like to display a commodities ticker in your own language. This can be easily done by specifying your custom name between parenthesis, right after you have specified the symbol. For example, you can create a commodities ticker in Spanish specifying the following in the symbols parameter: GC(Oro);SI(Plata);CL(Petr�leo Crudo). This works for any symbol, index, commodity or currency pair.

= Can I specify the numbers and dates format used in my country/region? =

Yes, Stockdio supports a number of cultures, used to properly display numbers and dates. For a complete list of cultures currently supported by Stockdio, please visit [www.stockdio.com/cultures](http://www.stockdio.com/cultures).

= Can I specify my own colors for the list? =

Yes, this plugin is provided with a number of predefined color palettes, for ease of use. For a complete list of color palettes currently supported by Stockdio, please visit [www.stockdio.com/palettes](http://www.stockdio.com/palettes). However, if you need specific color customization, you can use the Stock Quotes List block, or you can use the Stockdio iframe available at [http://services.stockdio.com](http://services.stockdio.com), which supports more options.

= Is the list data real-time or delayed? =

In most cases the data is delayed but the delay time may vary between 1 minute and 20 minutes, depending on the exchange. For details of intraday delay time for each exchange please visit [www.stockdio.com/exchanges](http://www.stockdio.com/exchanges).

= The company logo for one of the symbols is not correct or updated, can this be fixed? =

Sure! Simply contact us to info@stockdio.com with the correct or updated logo and we will update it, once it has been verified.

= Can I place more than one list on the same page? =

Yes. By default, all lists will use the values specified in the plugin settings page. However, any of these values can be overridden using the appropriate shortcode parameter. Each shortcode can be customized entirely independent.

= How can I contact Stockdio if something is not working as expected? =

Simply send an email to info@stockdio.com with your question and we will reply as soon as possible.

= Can I create a Cryptocurrencies list? =

Yes. You must use CRYPTO as the stockExchange and then specify one or more cryptocurrencies in the symbols parameter. For example, use BTC;ETH;LTC for Bitcoin, Ethereum and Litecoin. For a complete list of cryptocurrencies currently supported by Stockdio, please visit [www.stockdio.com/cryptocurrencies](https://www.stockdio.com/cryptocurrencies).

= Can I create a Futures list? =

Yes. You must use FUTURES as the stockExchange and then specify one or more futures in the symbols parameter. For example, use GCM19;QAG19;FXH19 for Gold, Brent Oil and Eurostoxx. For a complete list of futures currently supported by Stockdio, please visit [www.stockdio.com/futures/](https://www.stockdio.com/futures).

= Can I create a Bonds list? =

Yes. You must use BONDS as the stockExchange and then specify one or more bonds in the symbols parameter. For example, use US10YBY;UK10YBY; JA10YBY for US, UK and Japan's 10-Year Bond Yield. For a complete list of bonds currently supported by Stockdio, please visit [www.stockdio.com/bonds](https://www.stockdio.com/bonds)


== Screenshots ==

1. Example of quotes board used to display a World Markets Watch List.

2. Example of quotes board used to display a Commodities list, with interactive chart.

3. Example of quotes board used to display a World Currencies List, with interactive chart.

4. Example of quotes board using Financial motif and Financial-Light palette.

5. Example of quotes board using Face motif and Relief palette.

6. Example of quotes board using Material motif and Whitespace palette, using Spanish-Spain culture.

7. Example of quotes board using Semantic motif and Humanity palette, using French-Canada culture.

8. Example of quotes board using Blinds motif and Block palette, using German-Germany culture.

9. Example of quotes board using Healthy motif and Healthy palette, using Italian-Italy culture.

10. Example of quotes board using Block motif and Relief palette.

11. Stockdio Historical Chart is also available as a complement to the Stock Quotes List. 

12. Stockdio Stock Market Overview is also available as a complement to the Stock Quotes List. 

13. Stockdio Stock Market News is also available as a complement to the Stock Quotes List.

14. Stockdio Stock Market Ticker List is also available as a complement to the Stock Quotes List.

15. Settings page.

16. Stockdio toolbar integration with easy to use dialog.

17. Stock Quotes List widget dialog.

18. Stock Quotes List block as part of the Stockdio Financial Visualizations category.

19. Stock Quotes List block sidebar settings.

== Changelog ==
= 2.9.16 =
Release date: July 18, 2024

* Fixes issue with block editor.

= 2.9.15 =
Release date: May 29, 2024

* Fixes stock search issues.
* Fixes vulnerability issue.

= 2.9.14 =
Release date: May 09, 2024

* Fixes issue with Stock Exchange in Settings page.

= 2.9.13 =
Release date: March 07, 2024

* Fixes vulnerability issue.

= 2.9.12 =
Release date: March 05, 2024

* Fixes vulnerability issue.

= 2.9.11 =
Release date: November 01, 2023

* Fixes vulnerability issue.

= 2.9.10 =
Release date: October 20, 2023

* Fixes vulnerability issue.

= 2.9.9 =
Release date: March 30, 2023

* Minor bug fixes.

= 2.9.7 =
Release date: May 24, 2022

* Minor bug fixes.

= 2.9.6 =
Release date: March 01, 2022

* Minor bug fixes.

= 2.9.5 =
Release date: May 03, 2021

* Minor bug fixes.

= 2.9.4 =
Release date: January 27, 2021

* Minor bug fixes to properly support compatibility with legacy versions of WordPress.

= 2.9.3 =
Release date: January 24, 2021

* Minor block bug fixes and enhancements.

= 2.9.2 =
Release date: January 19, 2021

* Minor block bug fixes and enhancements.

= 2.9.1 =
Release date: January 14, 2021

* Addition of wizard to easily support selection of symbols.
* Minor bug fixes and security enhancements.

= 1.8.3 =
Release date: July 8, 2020

Bug Fixes:

* Fix of issue that displayed the wrong stock exchange at the front end.

= 1.8.2 =
Release date: June 19, 2020

Bug Fixes:

* Minor block bug fixes and enhancements.

= 2.8.1 =
Release date: June 18, 2020

* Addition of the Stock Market Ticker block for easy configuration in the standard Gutenberg editor.

= 2.7.15 =
Release date: May 7, 2020

* Change to support referrals on certain browsers

= 2.7.14 =
Release date: April 02, 2020

* Support for new culture: Traditional Chinese

= 2.7.13 =
Release date: December 09, 2019

* Fixes issue with Load Data When Visible setting.

= 2.7.12 =
Release date: August 16, 2019

* Support for NEO Exchange (NEO).

= 2.7.11 =
Release date: January 31, 2019

* Support for Cryptocurrencies, Futures and Bonds.
* Fixes issue with deprecated functions.

= 2.7.10 =
Release date: October 24, 2018

* Fixes issue with ticker auto calculated height.

= 2.7.9 =
Release date: October 03, 2018

* Support for new cultures: Turkish, Arabic, Hebrew, Swedish, Danish, Finnish, Norwegian, Icelandic, Greek, Czech, Thai, Vietnamese, Hindi, Indonesian

= 2.7.8 =
Release date: June 05, 2018
 
New features:
 
* Support for ability load data only when the visualization becomes visible. Please refer to the documentation for details.

= 2.7.6 =
Release date: May 14, 2018

* Fixes issue with deprecated functions.

= 2.7.4 =
Release date: November 30, 2017

* Support for WordPress 4.9

= 2.7.3 =
Release date: August 3, 2017

Bug Fixes:

* Fixes an issue that might cause some visualizations to appear cut off.

= 2.7.2 =
Release date: August 2, 2017

* Enhancements on mobile display.

= 2.7.1 =
Release date: June 21, 2017

Bug Fixes:

* Some properties in Settings page and shortcode were not being honored during plugin rendering.

= 2.7 =
Release date: June 12, 2017

* Support for BATS ETF (included in the NYSENasdaq stockExchange category).

= 2.6 =
Release date: May 25, 2017

* Support for Canadian Securities Exchange (CSE).
* Support for new language and culture: Polish-Poland.

= 2.5 =
Release date: May 12, 2017

New features:

* Ability to show currency symbol next to the price.
* End user can now sort the list by any displayed field (e.g. symbol, name, price, percent change, etc.)
* Stock Quotes List Widget is now available along with the plugin, for even easier integration. 

= 2.4 =
Release date: March 28, 2017

* Compatibility with new plugins Marketplace.

= 2.3 =
Release date: March 22, 2017

* Compatibility with new Stock Market Overview plugin.

= 2.2 =
Release date: March 1, 2017

* New Feature: ability to combine different stock exchanges, commodities and currencies on the same quote list. Refer to the FAQ for details.

= 2.1 =
Release date: February 24, 2017

* Support for new language and culture: Turkish-Turkey.
* Compatibility with new Stock Market Ticker plugin.
* Support of custom name for company/commodities/currencies.

= 2.0 =
Release date: November 30, 2016

* Support for auto refresh intraday delayed data, if available for the exchange. For a list of exchanges that support intraday data, visit http://www.stockdio.com/exchanges.
* Bug fix: solves an issue with "Call to undefined function com_create_guid()" that appears in some cases.
* Bug fix: solves an issue that wrongfully uses the palette name as title, in some cases.

= 1.2 =
Release date: November 10, 2016

* Support for interactive chart along with the list.
* Support for Currencies (Forex) and Commodities prices.

= 1.1.8 =
Release date: October 13, 2016

Support for several additional stock exchanges and their corresponding indices:

* Johannesburg Stock Exchange (JSE)
* Irish Stock Exchange (ISE)
* Tadawul Saudi Stock Exchange (TADAWUL)
* Warsaw Stock Exchange (WSE)
* Philippine Stock Exchange (PSE)
* Abu Dhabi Securities Exchange (ADX)
* Dubai Financial Market (DFM)
* Bolsa de Valores de Colombia (BVC)
* Taipei Exchange (TPEX)
* Bolsa de Valores de Lima (BVL)
* The Egyptian Exchange (EGX) 
* Nairobi Securities Exchange (NASE)
* Hanoi Stock Exchange (HNX)
* Ho Chi Minh Stock Exchange (HOSE)
* Prague Stock Exchange (BCPP)
* Amman Stock Exchange (AMSE)

= 1.1.7 =
Release date: August 22, 2016

Support for several additional stock exchanges and their corresponding indices:

* Borsa Istanbul (BIST) 
* NASDAQ OMX Tallinn (OMXT)
* NASDAQ OMX Riga (OMXR)
* NASDAQ OMX Vilnius (OMXV)
* Qatar Stock Exchange (QSE)
* Athens Stock Exchange (ASE)

= 1.1.6 =
Release date: August 19, 2016

Bug Fixes:

* Some properties were not being honored during plugin rendering unless the settings page was saved previously

= 1.1.5 =
Release date: August 5, 2016

New Features:

* Support for US Mutual Funds.

Bug Fixes:

* Symbols were not being saved in Settings page.
* Some properties in Settings page and shortcode were not being honored during plugin rendering.

= 1.1.4 =
Release date: August 1, 2016

Support for several additional stock exchanges and their corresponding indices:

* OTC Markets (OTCMKTS)
* OTC Bulletin Board (OTCBB)
* Vienna Stock Exchange/Wiener Boerse (VSE)
* Bolsa de Comercio de Santiago (BCS)

= 1.1.3 =
Release date: July 19, 2016

New Features:

* Ability to display market indices and even mix stocks and indices in the same list.
* Display index country flag as logo.
* Specify the maximum logo width and height, particularly useful for smaller fonts.

Support for several additional stock exchanges and their corresponding indices:

* New Zealand Exchange (NZX)
* Oslo Stock Exchange (OSE)
* Singapore Exchange (SGX)
* Stock Exchange of Thailand (SET)
* Bolsa de Comercio de Buenos Aires (BCBA)

= 1.1.2 =
Release date: July 7, 2016

* Support for Nigerian Stock Exchange (NGSE) 

= 1.1.1 =
Release date: July 5, 2016

* Support for Bursa Malaysia Stock Exchange (KLSE) 

= 1.1 =
Release date: June 28, 2016

* Support for Tel Aviv Stock Exchange (TASE).

= 1.0 =
* Initial version.

== Upgrade Notice ==
