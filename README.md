# Assignment-6.1
Numpy - Vander

import numpy as nm
x=nm.array(list(map(int,input("Enter the numbers: ").split(","))))
N=(len(x))
ans=nm.column_stack([x**(N-1-i) for i in range(N)])
print("Array is:")
print(ans)
checker=nm.vander(x, increasing=False)
print("applying numpy.vander to check, Array is: ")
print(checker)
