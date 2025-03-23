

### Switch

```
switch(expr) {
  case x:
  break;
  case y:
  break;
  case z:
  case a:
    break;
  default:
    
}
```


### Strings

Iterating through strings:

```
for (int i = 0; i < s.length(); i++) {
    char c = s.charAt(i);
}
```

StringBuilder
```
StringBuilder sb = new StringBuilder();
sb.append("Hello");

StringBuilder reverse = sb.reverse();

String result = reverse.toString();
```

Inteface for both StringBuilder and String:
```
CharSequence string; // Can pass both StringBuilder and String
```

### Stacks / Queue

```
Deque<Integer> stack = new ArrayDeque<>();

stack.push(); // Add to head of list.
stack.pop(); // Remove from head of list.

queue.remove(); 
queue.removeFirst(); // Remove from head of list

queue.add();
queue.addLast();  // Add to end of list.
```


### Heaps / Priority Queue

Min Heap
```
PriorityQueue<Integer> heap = new PriorityQueue<>(); // Default Collections.

heap.add(num); //add
heap.remove(); //(remove lowest)
heap.peek(); // Check but don't remove.

```

Max Heap
```
PriorityQueue<Integer> heap
            = new PriorityQueue<Integer>(
                Collections.reverseOrder());
```
PriorityQueue(int initialCapacity, Comparator<E> comparator)


Lambda comparator
```
PriorityQueue<Integer> heap = new PriorityQueue<Integer>((d1,d2) -> d1 - d2);
```

### Converting a Set to List and sorting, for each loop

```
Map<Ineger, List> columnValues = new ArrayList<>();
List<Integer> sortedKeys = new ArrayList<>(columnValues.keySet());
Collections.sort(sortedKeys);

for(int k: sortedKeys) {
    result.add(columnValues.get(k));
}
```

### Pairs
```
Pair<TreeNode, Integer> pair = new Pair<>(root, 0);
int node = pair.getKey();
int column = pair.getValue();
```

### Random

```
Math.random()
```

### Converting Integer to char array:
```
char[] numArr = Integer.toString(num).toCharArray();

in num = Integer.parseInt(String.valueOf(numArr));

```

### Case Character
```
Character.toLowerCase(c);
Character.toUpperCase(c);
```

### Case String
```
String s = "hello";
s.toUpperCase();
s.toLowerCase();
```

### Array
```
 int[] myArray = {1, 2, 3, 4, 5};
 ```
