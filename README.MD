Supported Exchange marketplaces  
  
Please read the exchange specific notes to learn about eventual, special configurations needed for each exchange.  
  
    Binance  
    Bittrex  
    FTX  
    Gate.io  
    Huobi  
    Kraken  
    OKX (Former OKEX)  
    potentially many others. (We cannot guarantee they will work)  
  
Community tested  
  
Exchanges confirmed working by the community:  
  
    Bitvavo  
    Kucoin  
  
 Based on Python 3.8+: For botting on any operating system - Windows, macOS and Linux.  
Persistence: Persistence is achieved through sqlite.  
Dry-run: Run the bot without paying money.  
Backtesting: Run a simulation of your buy/sell strategy.  
Strategy Optimization by machine learning: Use machine learning to optimize your buy/sell strategy parameters with real exchange data.  
Edge position sizing Calculate your win rate, risk reward ratio, the best stoploss and adjust your position size before taking a position for each specific market.  
Whitelist crypto-currencies: Select which crypto-currency you want to trade or use dynamic whitelists.  
Blacklist crypto-currencies: Select which crypto-currency you want to avoid.  
Builtin WebUI: Builtin web UI to manage your bot.  
Manageable via Telegram: Manage the bot with Telegram.  
Display profit/loss in fiat: Display your profit/loss in fiat currency.  
Performance status report: Provide a performance status of your current trades.    
  
Bot commands  
  
usage: freqtrade [-h] [-V]  
                 {trade,create-userdir,new-config,new-strategy,download-data,convert-data,convert-trade-data,list-data,backtesting,edge,hyperopt,hyperopt-list,hyperopt-show,list-exchanges,list-hyperopts,list-markets,list-pairs,list-strategies,list-timeframes,show-trades,test-pairlist,install-ui,plot-dataframe,plot-profit,webserver}
                 ...
  
Free, open source crypto trading bot  
  
positional arguments:  
  {trade,create-userdir,new-config,new-strategy,download-data,convert-data,convert-trade-data,list-data,backtesting,edge,hyperopt,hyperopt-list,hyperopt-show,list-exchanges,list-hyperopts,list-markets,list-pairs,list-strategies,list-timeframes,show-trades,test-pairlist,install-ui,plot-dataframe,plot-profit,webserver}  
    trade               Trade module.  
    create-userdir      Create user-data directory.  
    new-config          Create new config  
    new-strategy        Create new strategy  
    download-data       Download backtesting data.  
    convert-data        Convert candle (OHLCV) data from one format to
                        another.  
    convert-trade-data  Convert trade data from one format to another.  
    list-data           List downloaded data.  
    backtesting         Backtesting module.  
    edge                Edge module.  
    hyperopt            Hyperopt module.  
    hyperopt-list       List Hyperopt results  
    hyperopt-show       Show details of Hyperopt results  
    list-exchanges      Print available exchanges.  
    list-hyperopts      Print available hyperopt classes.  
    list-markets        Print markets on exchange.  
    list-pairs          Print pairs on exchange.  
    list-strategies     Print available strategies.  
    list-timeframes     Print available timeframes for the exchange.  
    show-trades         Show trades.  
    test-pairlist       Test your pairlist configuration.  
    install-ui          Install FreqUI  
    plot-dataframe      Plot candles with indicators.  
    plot-profit         Generate plot showing profits.  
    webserver           Webserver module.  

optional arguments:  
  -h, --help            show this help message and exit  
  -V, --version         show program's version number and exit  

Telegram RPC commands  

Telegram is not mandatory. However, this is a great way to control your bot. More details and the full command list on the documentation  

    /start: Starts the trader.  
    /stop: Stops the trader.  
    /stopbuy: Stop entering new trades.  
    /status <trade_id>|[table]: Lists all or specific open trades.  
    /profit [<n>]: Lists cumulative profit from all finished trades, over the last n days.  
    /forceexit <trade_id>|all: Instantly exits the given trade (Ignoring minimum_roi).  
    /fx <trade_id>|all: Alias to /forceexit  
    /performance: Show performance of each finished trade grouped by pair  
    /balance: Show account balance per currency.  
    /daily <n>: Shows profit or loss per day, over the last n days.  
    /help: Show help message.  
    /version: Show version.  
