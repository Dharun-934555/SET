                                                     # SET #
                    ### "LIFE IS LIKE A PYTHON SET: NO DUPLICATES ALLOWED, BUT INTERSECTIONS MAKE IT  INTERESTING." ### 
INTRODUCTION :
       🍀 A set is a group of unique things kept together.
       🍀 It does not allow duplicates (same item cannot repeat).
       🍀 The order of items in a set does not matter.
👉 Example:
        A set of fruits = {apple, banana, mango}
        
TYPES OF SET :
      ✨Empty Set (Null Set)       
      ✨Finite Set
      ✨Infinite Set
      ✨Subset
      ✨Proper Subset
      ✨Universal Set
      ✨Disjoint Sets

TYPES OF METHOD :
🌸 add() – Add one item
      s = {1, 2}
      s.add(3)
      print(s)        # {1, 2, 3}

🌸 update() – Add many items
      s = {1, 2}
      s.update([3, 4])
      print(s)          # {1, 2, 3, 4}

🌸 remove() – Remove item (error if not found)
       s = {1, 2, 3}
       s.remove(2)
       print(s)         # {1, 3}

🌸 discard() – Remove item (no error if not found)
      s = {1, 2, 3}
      s.discard(5)  
      print(s)          # {1, 2, 3}

🌸 union() – Combine sets
      a = {1, 2}
      b = {2, 3}
      print(a.union(b))  # {1, 2, 3}

🌸 intersection() – Common items
      a = {1, 2, 3}
      b = {2, 3, 4}
      print(a.intersection(b))  # {2, 3}

🌸 difference() – Items only in one set
      a = {1, 2, 3}
      b = {2, 3}
      print(a.difference(b))   # {1}

🌸 symmetric_difference() – Items not common
      a = {1, 2, 3}
      b = {3, 4}
      print(a.symmetric_difference(b))   # {1, 2, 4}

🌸issubset() – Check smaller set
      a = {1, 2}
      b = {1, 2, 3}
      print(a.issubset(b))   # True

🌸issuperset() – Check bigger set
      a = {1, 2, 3}
      b = {1, 2}
      print(a.issuperset(b))   # True


# EXERCISE 1 : 

1. Find the length of the set it_companies
2. Add 'Twitter' to it_companies
3. Insert multiple IT companies at once to the set it_companies
4. Remove one of the companies from the set it_companies
5. What is the difference between remove and discard

# EXERCISE 2 :
1. Join A and B
2. Find A intersection B
3. Is A subset of B
4. Are A and B disjoint sets
5. Join A with B and B with A
6. What is the symmetric difference between A and B
7. Delete the sets completely

 # IMPLEMENTATION :
 
# EXERCISE 1 :

it_companies = {'Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Oracle', 'Amazon'}
A = {19, 22, 24, 20, 25, 26}
B = {19, 22, 20, 25, 26, 24, 28, 27}
age = [22, 19, 24, 25, 26, 24, 25, 24]
print(len(it_companies))

it_companies.add('Twitter')
print(it_companies)

it_companies.update('Infosys','Zoho','Ey')
print(it_companies)

it_companies.remove('Apple')
print(it_companies)

# EXERCISE 2 :

a = {'apple','orange','banana'}
b = {'potato','ladiesfinger','tomato','banana','apple'}

A = a & b
print(A)

a.update(b)
print(a)

if a.issubset(b):
  print('True')
else:
  print('False')

if a.isdisjoint(b):
  print('True')
else:
  print('False')
  
a.union(b)
print(a)

b.union(a)
print(b)

b = {'apple','orange','banana'}
a = {'potato','ladiesfinger','tomato','banana','apple'}

a.symmetric_difference(b)
print(a)

del A


# OUTPUT :
7
{'Oracle', 'Google', 'Twitter', 'Amazon', 'Facebook', 'IBM', 'Microsoft', 'Apple'}
{'y', 'Z', 'Apple', 'Oracle', 'Google', 'Twitter', 'Facebook', 'I', 'E', 'h', 's', 'IBM', 'n', 'f', 'o', 'Amazon', 'Microsoft'}
{'y', 'Z', 'Oracle', 'Google', 'Twitter', 'Facebook', 'I', 'E', 'h', 's', 'IBM', 'n', 'f', 'o', 'Amazon', 'Microsoft'}
{'banana', 'apple'}
{'ladiesfinger', 'orange', 'tomato', 'potato', 'banana', 'apple'}
False
False
{'ladiesfinger', 'orange', 'tomato', 'potato', 'banana', 'apple'}
{'ladiesfinger', 'tomato', 'potato', 'banana', 'apple'}
{'ladiesfinger', 'tomato', 'potato', 'banana', 'apple'} 

          ### Thank you for visiting this repo! May your code always run without errors, your bugs be as rare as duplicates in a Python set, and your life full of meaningful intersections.


