# ECE2112---ADVANCED-PROGRAMMING---PA2
This project demonstrates the use of NumPy in solving two problems:

# Normalization Problem
- Generate a random 5x5 matrix.
- Apply normalization using the formula:

        Z = X - Xˉ​/σ

where: 
   - Xˉ​ is the mean of the data.
   - σ is the standard deviation of the data.
- The normalized values are stored in a .npy file for later use.

# Divisible by 3 Problem
- Create a 10x10 matrix containing the squares of the first 100 positive integers.
- Extract all elements that are divisible by 3.
- Save the extracted elements as a .npy file.

# Requirements 
- Python 3.8+
- NumPy
Install NumPy with:
pip install numpy

# How to Run
1. Run the Normalization Problem script:
        python normalization.py
- This will create and save X_normalized.npy.

2. Run the Divisible by 3 Problem script:
        python divisible_by_3.py
- This will create and save divby3.npy.
3. To load the saved files later:
        import numpy as np

        Xnorm = np.load("X_normalized.npy")
        divby3 = np.load("divby3.npy")

        print(Xnorm)
        print(divby3)

# Outputs
- X_normalized.npy → Normalized 5×5 matrix.
- divby3.npy → 1D array of numbers (from squares 1–100) divisible by 3.
