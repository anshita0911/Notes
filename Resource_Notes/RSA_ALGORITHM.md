# **RSA ALGORITHM:**

> **Key Generation:**

1. ## **Select two huge primes numbers**

   $ p \: \mathbb{and} \: q $

2. ## **Calculate**

   $​ n = p \times q $

3. ## **Calculate Euler's Totient Function**

   $ \varphi (n) = (p-1) \times (q-1) $

4. ## **Choose the value of e such that**

   $ d \equiv e^{-1} \bmod \varphi(n) \rightarrow ed \bmod \varphi(n) = 1 $

5. ## **Public Key**

   $ ​\{e,n\} $

6. ## **Private Key**

   $ \{d,n\} $