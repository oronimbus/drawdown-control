# Trade Sizing and Drawdown Control

This example notebook is trying to replicate some of the results from the Strub (2021) paper on Drawdown Control. The results are purely hypothetic and should not be used for financial decision making.

## Usage
- Make sure you install the following dependencies: `pip install numpy scipy pandas arch tqdm matplotlib yfinance`
- Execute the `drawdown-control.ipynb` notebook from top to bottom
- One step in the calculation takes a long time to execute (almost 2 hours), hence I've added a pickled dump of the data set which can be loaded by running:

```python
import pickle
with open("data/evt_results.pk", "rb") as file:
    results = pickle.load(file)
```

Note that this was put together in a single morning so I'm happy for any comments or criticism. Sharing is caring :-)

## References
Strub, Issam S., Trade Sizing Techniques for Drawdown and Tail Risk Control (May 21, 2016). Available at SSRN: https://ssrn.com/abstract=2063848