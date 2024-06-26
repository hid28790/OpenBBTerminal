---
title: fib
description: Discover how to calculate fibonacci retracement levels with our flexible
  parameters. Perfect for financial analysts and traders.
keywords:
- fib
- fibonacci retracement
- financial tool
- trading
- parameters
---

import HeadTitle from '@site/src/components/General/HeadTitle.tsx';

<HeadTitle title="forex/ta/fib - Reference | OpenBB Terminal Docs" />

Calculates the fibonacci retracement levels

### Usage

```python
fib [-p PERIOD] [--start START] [--end END]
```

---

## Parameters

| Name | Description | Default | Optional | Choices |
| ---- | ----------- | ------- | -------- | ------- |
| period | Days to look back for retracement | 120 | True | range(1, 960) |
| start | Starting date to select | None | True | None |
| end | Ending date to select | None | True | None |

![fib](https://user-images.githubusercontent.com/46355364/154310727-81a1eab3-5565-42c7-8b47-4f80288dd700.png)

---
