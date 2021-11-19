### Chicago Board of Trade (CBOT)

1. Load and read file:

```
import pandas as pd
df = pd.read_csv('https://raw.githubusercontent.com/ivanfilhoreis/agricultural_commodity_data/main/CBOT/corn.csv', 
                 delimiter=',', 
                 index_col='Date')
df.head()
```

<p align="center">
  <img src="https://github.com/ivanfilhoreis/agricultural_commodity_data/blob/main/CBOT/img/head_corn.png?raw=true" width="400px" alt="table2"/>
</p>

## 🔎 References

* [Markers Businness Insider](https://markets.businessinsider.com/commodities/soybeans-price)
 

