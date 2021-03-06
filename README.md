# Quandl Api

#### A repo of scripts for pulling data from the Quandl Api.

<code>$ py [filename].py</code>

##### QuandlFuturesVix.py

This python script collects the settle and close price of each
futures contract. Then it appends the contract name and collects the
close price from the VIX Index. The data is then combined in
a pandas DataFrame and exported to files
<code>data/[date]_quandl_futures_vix.[ext]</code>

##### FieldsDaily.py

This python script collects data from six indexes related to Volatility:
VXST, VIX, VXV, VX1, VX2, and VXMT.
This data is exported to files
<code>data/[date]_fields_daily.[ext]</code>

##### TermStructureIndicators.py

This python script uses the data produced from FieldsDaily.py to calculate:
VDelta, Roll Yield, Contango, Contango Roll, VRatio, VXV Roll, and VCO.
The data is exported to files
<code>data/[data]_term_structure_indicators.[ext]</code>
