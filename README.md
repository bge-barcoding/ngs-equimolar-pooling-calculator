# NGS Equimolar Pooling Calculator

A web-based tool for calculating equimolar pooling volumes from complex sub-pools for Next-Generation Sequencing (NGS).

## About

This calculator helps researchers determine the correct volumes to take from each pool when combining multiple complex sub-pools of NGS libraries for sequencing. It ensures that each individual sample contributes an equal number of molecules to the final sequencing run, resulting in more balanced coverage.

## Features

- Calculate equimolar pooling volumes for any number of input pools
- Support for both calculated (estimated / target) and measured concentrations
- Option to maximize the usage of original pools
- Adjustable final volume
- Real-time results with detailed metrics
- Verification of equimolarity across samples

## Live Calculator

The calculator is available at: https://bwprice.github.io/ngs-equimolar-pooling-calculator/

## Usage

1. Enter information for each input pool:
   - Molarity that each sample was normalized to in the sub-pool - i.e. the target molarity when pooling (nM)
   - Total pool volume (μl)
   - Number of samples in the pool
   - (Optional) Measured concentration of each sub-pool from lab quantification

2. Choose whether to:
   - Use measured concentrations (if available from Qubit, Bioanalyzer, qPCR, etc.)
   - Maximize usage of original pools
   - Set a specific final pool volume

3. The calculator will automatically determine:
   - How much volume to take from each sub-pool
   - The percentage of each sub-pool that will be used
   - The final nM contribution per sample
   - Total samples in the final pool

## Installation for Local Development

1. Clone this repository:
   ```
   git clone https://github.com/bwprice/ngs-equimolar-pooling-calculator.git
   cd ngs-equimolar-pooling-calculator
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Start the development server:
   ```
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

## Deployment

To deploy to GitHub Pages:

```
npm run deploy
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Citation

If you use this tool in your research, please cite:

```
Ben Price (2025) NGS Equimolar Pooling Calculator, GitHub Repository, 
Available at: https://github.com/bwprice/ngs-equimolar-pooling-calculator
```
