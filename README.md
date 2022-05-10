class Solution:
    def countPrimes(self, n: int) -> int:
        primes = [True for i in range(n)]
        i = 2
        while(i*i < n):
            i += 1
        
        counter = 0
        for i in range(2, len(primes)):
            if primes[i]:
                counter += 1
        return counter
