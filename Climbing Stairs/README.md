这道题非常有意思。每次可以爬 1-2 阶。

那么一开始的想法是，总的数量

f(n) = ∑C(i,n-1), i from 0 to floor(n/2)

公式推出来的时间复杂度大约是 O(n(n/2)!)：

1+(n-1)+(n-2)(n-3)/2!+(n-3)(n-4)(n-5)/3!+(n-4)(n-5)(n-6)(n-7)/4!+...+1

经过简化后的时间复杂度大约是 O(n^2)（原因是阶乘）

------

然后惊讶地发现

f(4)=5, f(5)=8, f(6)=13...

这货竟然是斐波那契序列！！！！

这说明了

f(n) = f(n-1) + f(n-2)

------

恍然大悟！

于是其时间复杂度为 O(n^2)（原因是大数加法）

并且，如果通过通项公式求解，时间复杂度为 O(1)

------

wikipedia 上找到的起源：
The Fibonacci sequence appears in Indian mathematics, in connection with Sanskrit prosody.[8][13] In the Sanskrit tradition of prosody, there was interest in enumerating all patterns of long (L) syllables that are 2 units of duration, and short (S) syllables that are 1 unit of duration. Counting the different patterns of L and S of a given duration results in the Fibonacci numbers
