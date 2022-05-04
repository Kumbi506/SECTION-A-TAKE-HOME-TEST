# SECTION-A-TAKE-HOME-TEST HYPERIONDEV
CODE REVIEW FOR PYTHON CODE

I have noted the following in the code given below
-The code uses a class. I think a function will suffice.
- The code does not run. It presented a lot of errors on running.
- The class is not initialised with the `def __init__` initialiser.
- The code is not efficient.

Here is the given code

```Python
class Solution:
       def groupAnagrams(self, strs):
      result = {}
      for i in strs:
         x = "".join(sorted())
         if x in result:
            result[x].append(i)
         else:
            result[x] = [i]
      return list(result.values())
ob1 = Solution()
print(ob1.groupAnagrams(["eat", "tea", "tan", "ate", "nat", "bat"]))
```
Here is my corrected code which ran

```Python
def groupAnagrams(strs):
      result = {}
      for i in strs:
         x = str(sorted(i))
         if x in result:
            result[x].append(i)
         else:
            result[x] = [i]
      return list(result.values())

print(groupAnagrams(["eat", "tea", "tan", "ate", "nat", "bat"]))
```
The code is much shorter than the given one and it does run
