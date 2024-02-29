# Better Period Separators MT5

This code is a customizable period separator tool for MetaTrader 5 (MT5) platform, developed by the Forex Robot Easy Team. It allows users to determine the period separators and create personalized separators for better flexibility and usability.

## Features

1. Customizable Period Separators:
   - Enable users to determine the period for better flexibility.
   - Implement the ability to create personalized period separators.
   - Enhance the usability of the MT5 platform.

2. Specific Time Placement for Intraday Charts:
   - Cater to the needs of intraday traders.
   - Allow users to place period separators at a specific time.
   - Provide the option to insert additional period separators.

## Usage

### Initialization

The expert initialization function `OnInit()` sets the period separators using the `SetPeriodSeparators()` function.

### Deinitialization

The expert deinitialization function `OnDeinit()` removes the period separators using the `RemovePeriodSeparators()` function.

### Setting Period Separators

The `SetPeriodSeparators()` function defines the period separators by specifying the datetime values for custom separators. In this code, two custom separators are defined as `separator1` and `separator2`, set to `2022.01.01 00:00:00` and `2022.03.01 00:00:00` respectively. The `ChartSetInteger()` function is then used to set the period separators on the chart.

### Removing Period Separators

The `RemovePeriodSeparators()` function removes all period separators by setting the `CHART_PERIOD_SEPARATOR` property to zero.

### Placing Additional Period Separators

In the `OnTick()` function, you can place your trading logic. If a specific time placement is required, you can use the `InsertPeriodSeparator()` function. In this code, the function is called if the current time is 12:00 (noon). It inserts an additional period separator at that specific time using the `ChartSetInteger()` function.

### Inserting Additional Period Separator

The `InsertPeriodSeparator()` function inserts an additional period separator at the specified time. It uses the `ChartSetInteger()` function with the `CHART_PERIOD_SEPARATOR` property.

## Product Description

This code provides a customizable period separator tool for MetaTrader 5 (MT5) platform, developed by the Forex Robot Easy Team. It allows users to determine the period separators and create personalized separators for better flexibility and usability.

With this tool, traders can easily set period separators according to their trading preferences. They can define custom separators at specific dates and times, enhancing the visualization of different trading periods on the chart.

Intraday traders can benefit from the ability to place period separators at specific times, such as the start or end of a trading session. This helps them analyze and identify trading opportunities within specific timeframes more effectively.

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that demonstrates how the product works. To find the official developer of this product and access detailed reviews and trading results, please refer to the following link: [Better Period Separators MT5 Review](https://forexroboteasy.com/forex-robot-review/better-period-separators-mt5-review-customizable-forex-trading-tool/).
