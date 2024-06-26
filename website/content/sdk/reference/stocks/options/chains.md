---
title: chains
description: This page provides comprehensive instructions on how to get option chain
  for a stock using openbb.stocks.options API. It provides examples including how
  to retrieve data from 'Nasdaq' and fetch specific expiration dates.
keywords:
- stock options
- option chain
- openbb.stocks.options.api
- Nasdaq
- expiration dates
- stock market API
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="stocks.options.chains - Reference | OpenBB SDK Docs" />

Get Option Chain For A Stock.  No greek data is returned

Source Code: [[link](https://github.com/OpenBB-finance/OpenBBTerminal/tree/main/openbb_terminal/stocks/options/options_sdk_helper.py#L20)]

```python
openbb.stocks.options.chains(symbol: str, source: str = "Nasdaq", expiration: Optional[str] = None)
```

---

## Parameters

| Name | Type | Description | Default | Optional |
| ---- | ---- | ----------- | ------- | -------- |
| symbol | str | Symbol to get chain for | None | False |
| source | str | Source to get data from, by default "Nasdaq" | Nasdaq | True |
| expiration | Union[str, None] | Date to get chain for.  By default returns all dates | None | True |


---

## Returns

| Type | Description |
| ---- | ----------- |
| pd.DataFrame | Dataframe of full option chain. |
---

## Examples

```python
from openbb_terminal.sdk import openbb
aapl_option_chain = openbb.stocks.options.chains("AAPL", source = "Nasdaq")
```

```
To get a specific expiration date, use the expiration parameter
```
```python
aapl_chain_date = openbb.stocks.options.chains("AAPL", expiration="2023-07-21", source="Nasdaq")
```

---
