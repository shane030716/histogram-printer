# Histogram Printer

HistogramPrinter prints out a histogram represented by an array of non-negative integers, 
where each integer in the array represents the height of each bar.

It's useful for debugging problems involving histograms. See [Largest Rectangle in a Histogram](https://github.com/shane030716/programming-problems#largest-rectangle-in-a-histogram) and [Volume of Histogram](https://github.com/shane030716/programming-problems#volume-of-histogram)

*(Note: this repository is a submodule of the the [programming-problems](https://github.com/shane030716/programming-problems/tree/master/src/util) repository.)*

This class has three public APIs so far

`printHistogram(int[] arr)`

Example: 

input: `[1,0,0,0,6,0,0,3,10,2,3,4,5,0,3,0]`

Output: 
```
                                 ___                            
                                |   |                           
                                |   |                           
                                |   |                           
                 ___            |   |                           
                |   |           |   |            ___            
                |   |           |   |        ___|   |           
                |   |        ___|   |    ___|   |   |    ___    
                |   |       |   |   |___|   |   |   |   |   |   
 ___            |   |       |   |   |   |   |   |   |   |   |   
|___|___ ___ ___|___|___ ___|___|___|___|___|___|___|___|___|___
  1   0   0   0   6   0   0   3  10   2   3   4   5   0   3   0
```  
`printWaterFilledHistogram(int[] arr)`

Image pouring water into the histogram, what is the maximum amount water it can hold.

Example: 

input: `[1,0,0,0,6,0,0,3,10,2,3,4,5,0,3,0]`

Output: (+ represents water)
```
                                 ___                            
                                |   |                           
                                |   |                           
                                |   |                           
                 ___            |   |                           
                |   |+++ +++ +++|   |            ___            
                |   |+++ +++ +++|   |+++ +++ ±±±|   |           
                |   |+++ +++ ±±±|   |+++ ±±±|   |   |    ___    
                |   |+++ +++|   |   |±±±|   |   |   |+++|   |   
 ___            |   |+++ +++|   |   |   |   |   |   |+++|   |   
|___|±±± ±±± ±±±|___|±±± ±±±|___|___|___|___|___|___|±±±|___|___
  1   0   0   0   6   0   0   3  10   2   3   4   5   0   3   0
```

`printLargestRectangleFilledHistogram(int[] arr)`

Fill the largest rectangle area that is can be formed by a number of contiguous bars, assuming the width of each bar is 1

Example: 

input: `[1,0,0,0,6,0,0,3,10,2,3,4,5,0,3,0]`

Output: (+ represents the filled area)
```
                                 ___                            
                                |   |                           
                                |   |                           
                                |   |                           
                 ___            |   |                           
                |   |           |   |            ___            
                |   |           |   |        ___|   |           
                |   |        ___|   |    ___|   |   |    ___    
                |   |       |   |   |___|   |   |   |   |   |   
 ___            |   |       |+++|+++|+++|+++|+++|+++|   |   |   
|___|___ ___ ___|___|___ ___|±±±|±±±|±±±|±±±|±±±|±±±|___|___|___
  1   0   0   0   6   0   0   3  10   2   3   4   5   0   3   0 
```

More features may be added in the future.
