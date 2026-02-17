# Assignment 1: Learning Probability Density Function using Roll Number Parameterized Model

## Dataset
India Air Quality Dataset
Feature used: NO2

## Roll Number
102303544

## Methodology

Step 1: Load the dataset using pandas.

Step 2: Select NO2 column as feature x and remove missing values.

Step 3: Calculate parameters using roll number:

a_r = 0.05 × (r mod 7)
b_r = 0.3 × (r mod 5 + 1)

For roll number 102303544:

a_r = 0
b_r = 1.5

Step 4: Transform data using transformation function:

z = x + a_r sin(b_r x)

Since a_r = 0:

z = x

Step 5: Estimate PDF parameters using statistical estimation:

μ = mean(z)
σ² = variance(z)
λ = 1 / (2σ²)
c = 1 / √(2πσ²)

## Results

μ = 25.809622897811263

λ = 0.001460436525489001

c = 0.021560876239314915

## Result Graph

Histogram and estimated PDF curve plotted using matplotlib.

## Conclusion

The probability density function parameters were successfully estimated using roll number parameterized transformation and statistical estimation technique.
