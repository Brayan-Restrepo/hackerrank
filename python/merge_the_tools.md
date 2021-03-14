### Merge the Tools!



Ref: [Hackerrank](https://www.hackerrank.com/challenges/merge-the-tools/problem)



```python
import collections

def merge_the_tools(string, k):
    n = round(len(string)/k)
    ni = 0
    nk = k
    for i in range(n):
        u = collections.OrderedDict.fromkeys(string[ni:nk]).keys()
        print(''.join(u))
        ni += k
        nk += k
    
    
if __name__ == '__main__':
    string, k = input(), int(input())
    merge_the_tools(string, k)
```
