# Hedge_SP500

Finding the optimal hedge of S&P500 using gold and bonds in different economic regimes.

## Optimization

Assumptions:

- Optimization Goal: Maximise Sharpe and Beat Market Returns
- Risk-Free Rate is 0
- Range of Possible Hedge Positions for Gold and Bonds: -1 to 1
- Threshold for determining gdp (rising/falling) is 2
- Threshold for determining cpi (rising/falling) is 2
- Modified Duration of a 10-Year Bond is 8

Economic Regime

- Goldilocks - Rising GDP and Falling Inflation
- Slow Growth - Slowing GDP and Falling Inflation
- Stagflation - Slowing GDP and Rising Inflation
- Heating Up - Rising GDP and Rising Inflation

#### Goldilocks

Optimized Weights (Gold, Bonds): ['0.371', '0.059']  
Achieved Annual Sharpe Ratio: 0.77  
Achieved Average Daily Return: 0.06 %

#### Goldilocks - Out-of-Sample Analysis

Weights (Gold, Bonds): ['0.371', '0.059']  
Achieved Annual Sharpe Ratio: 0.47  
Achieved Average Daily Return: 0.04 %

#### Heating Up

Optimized Weights (Gold, Bonds): ['0.672', '-0.050']  
Achieved Annual Sharpe Ratio: 1.08  
Achieved Average Daily Return: 0.08 %

#### Heating Up - Out-of-Sample Analysis

Weights (Gold, Bonds): ['0.672', '-0.050']  
Achieved Annual Sharpe Ratio: 0.41  
Achieved Average Daily Return: 0.05 %

#### Slow Growth

Optimized Weights (Gold, Bonds): ['1.000', '0.019']  
Achieved Annual Sharpe Ratio: 0.58  
Achieved Average Daily Return: 0.08 %

#### Slow Growth - Out-of-Sample Analysis

Weights (Gold, Bonds): ['1.000', '0.019']  
Achieved Annual Sharpe Ratio: 0.71  
Achieved Average Daily Return: 0.07 %

#### Stagflation

Optimized Weights (Gold, Bonds): ['1.000', '-0.086']  
Achieved Annual Sharpe Ratio: 0.57  
Achieved Average Daily Return: 0.09 %

#### Stagflation - Out-of-Sample Analysis

Weights (Gold, Bonds): ['1.000', '-0.086']  
Achieved Annual Sharpe Ratio: 0.64  
Achieved Average Daily Return: 0.08 %
