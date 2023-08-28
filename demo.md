


## Iterator interface

Iterator interface provides the facility of iterating the elements in a forward direction only.

Methods of Iterator interface

There are only three methods in the Iterator interface. 


|**No.**|**Method**|**Description**|
| :- | :- | :- |
|1|public boolean hasNext()|It returns true if the iterator has more elements otherwise it returns false.|
|2|public Object next()|It returns the element and moves the cursor pointer to the next element.|
|3|public void remove()|It removes the last elements returned by the iterator. It is less used.|



**List Interface in Java** 

The List interface in Java provides a way to store the ordered collection. It is a child interface of Collection. It is an ordered collection of objects in which duplicate values can be stored. Since List preserves the insertion order, it allows positional access and insertion of elements. 

The List interface is found in java.util package and inherits the Collection interface. It is a factory of the ListIterator interface. Through the ListIterator, we can iterate the list in forward and backward directions. The implementation classes of the List interface are ArrayList, LinkedList, Stack, and Vector. ArrayList and LinkedList are widely used in Java programming.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.002.png)










![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.003.jpeg)**What is ArrayList in Java?**

ArrayList is a Java class implemented using the List interface. Java ArrayList, as the name suggests, provides the functionality of a dynamic array where the size is not fixed as an array. Also as a part of the Collection framework, it has many features not available with arrays. 

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.004.png)




**Constructors in ArrayList**

In order to create an ArrayList, we need to create an object of the ArrayList class. The ArrayList class consists of various constructors which allow the possible creation of the array list. The following are the constructors available in this class:

1\. ArrayList()

This constructor is used to build an empty array list. If we wish to create an empty ArrayList with the name arr, then, it can be created as:

ArrayList arr = new ArrayList(); 

2\. ArrayList(Collection c)

This constructor is used to build an array list initialized with the elements from the collection c. Suppose, we wish to create an ArrayList arr which contains the elements present in the collection c, then, it can be created as: 

ArrayList arr = new ArrayList(c);  

3\. ArrayList(int capacity)

This constructor is used to build an array list with the initial capacity being specified. Suppose we wish to create an ArrayList with the initial size being N, then, it can be created as:

ArrayList arr = new ArrayList(N);

**Important Features of ArrayList in Java**

- ArrayList inherits AbstractList class and implements the List interface.
- ArrayList is initialized by size. However, the size is increased automatically if the collection grows or shrinks if the objects are removed from the collection.
- Java ArrayList allows us to randomly access the list.
- ArrayList can not be used for primitive types, like int, char, etc. We need a wrapper class for such cases.
- ArrayList is not Synchronized. Its equivalent synchronized class in Java is Vector.








**LinkedList in Java**

Java LinkedList class uses a doubly linked list to store the elements. It provides a linked-list data structure. It inherits the AbstractList class and implements List and Deque interfaces.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.005.png)**Hierarchy of LinkedList class**












**The important points about Java LinkedList are:**

o	Java LinkedList class can contain duplicate elements.

o	Java LinkedList class maintains insertion order.

o	Java LinkedList class is non synchronized.

o	In Java LinkedList class, manipulation is fast because no shifting needs to occur.

o	Java LinkedList class can be used as a list, stack or queue.

**How Does LinkedList work Internally?**

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.006.png)










**Constructors in the LinkedList:**

In order to create a LinkedList, we need to create an object of the LinkedList class. The LinkedList class consists of various constructors that allow the possible creation of the list. The following are the constructors available in this class:

1\. LinkedList(): This constructor is used to create an empty linked list. If we wish to create an empty 

LinkedList ll = new LinkedList();  

2\. LinkedList(Collection C): This constructor is used to create an ordered list that contains all the elements of a specified collection, as returned by the collection’s iterator. If we wish to create a LinkedList with the name ll, then, it can be created as: 

LinkedList ll = new LinkedList(C);

**Advantages of using LinkedList in Java:**

- Dynamic size: As with Vector, the size of a LinkedList can grow or shrink dynamically, so you don’t have to worry about setting an initial size.
- Efficient Insertions and Deletions: LinkedList is an efficient data structure for inserting or deleting elements in the middle of the list because you only need to change the links between elements, rather than shifting all elements after the insertion or deletion point.
- Flexible Iteration: With a linked list, you can efficiently iterate through the list in either direction, since each element has a reference to both its predecessor and successor elements.

**Disadvantages of using LinkedList in Java:**

- Performance: LinkedList has a slower performance than ArrayList when it comes to accessing individual elements. This is because you need to traverse the list to reach the desired element, whereas with ArrayList, you can simply access the desired element using an index.
- Memory overhead: LinkedList requires more memory than ArrayList because each element requires additional memory for the links to its predecessor and successor elements.













**Vector Class** 

The Vector class implements a growable array of objects. Vectors fall in legacy classes, but now it is fully compatible with collections. It is found in java.util package and implement the List interface, so we can use all the methods of the List interface as shown below as follows:

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.007.png)











**It is similar to the ArrayList, but with two differences**

- Vector is synchronized.
- Java Vector contains many legacy methods that are not the part of a collections framework.

**Constructors**

1\. Vector(): Creates a default vector of the initial capacity is 10.

Vector<E> v = new Vector<E>();

2\. Vector(int size): Creates a vector whose initial capacity is specified by size.

Vector<E> v = new Vector<E>(int size);

3\. Vector(int size, int incr): Creates a vector whose initial capacity is specified by size and increment is specified by incr. It specifies the number of elements to allocate each time a vector is resized upward.

Vector<E> v = new Vector<E>(int size, int incr);

4\. Vector(Collection c): Creates a vector that contains the elements of collection c.

Vector<E> v = new Vector<E>(Collection c);

**Advantages of using Vector in Java:**

- Synchronization: As mentioned before, Vector is synchronized, making it safe to use in a multi-threaded environment.
- Dynamic Size: The size of a Vector can grow or shrink dynamically as elements are added or removed, so you don’t have to worry about setting an initial size that will accommodate all elements.
- Legacy support: Vector has been part of Java since its inception and is still supported, so it’s a good option if you need to work with older Java code that uses Vector.

**Java Stack**

The stack is a linear data structure that is used to store the collection of objects. It is based on Last-In-First-Out (LIFO). Java collection framework provides many interfaces and classes to store the collection of objects. One of them is the Stack class that provides different operations such as push, pop, search, etc..

The stack data structure has the two most important operations that are push and pop. The push operation inserts an element into the stack and pop operation removes an element from the top of the stack. Let's see how they work on stack.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.008.png)













Let's push 20, 13, 89, 90, 11, 45, 18, respectively into the stack.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.009.png)







**Java Stack Class**

In Java, Stack is a class that falls under the Collection framework that extends the Vector class. It also implements interfaces List, Collection, Iterable, Cloneable, Serializable. It represents the LIFO stack of objects. Before using the Stack class, we must import the java.util package. The stack class arranged in the Collections framework hierarchy, as shown below.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.010.png)





















**Stack Class Constructor**

The Stack class contains only the default constructor that creates an empty stack.

public Stack()  

**Creating a Stack**

If we want to create a stack, first, import the java.util package and create an object of the Stack class.

Stack stk = new Stack(); 

` `Or

Stack<type> stk = new Stack<>();  

**Methods in stack**

|methods|modifier|discription|
| :- | :- | :- |
|[empty()](https://www.javatpoint.com/java-stack#empty)|boolean|The method checks the stack is empty or not.|
|[push(E item)](https://www.javatpoint.com/java-stack#push)|E|The method pushes (insert) an element onto the top of the stack.|
|[pop()](https://www.javatpoint.com/java-stack#pop)|E|The method removes an element from the top of the stack and returns the same element as the value of that function.|
|[peek()](https://www.javatpoint.com/java-stack#peek)|E|The method looks at the top element of the stack without removing it.|
|[search(Object o)](https://www.javatpoint.com/java-stack#search)|int|The method searches the specified object and returns the position of the object.|


**Set in Java**

The set interface is present in java.util package and extends the Collection interface. It is an unordered collection of objects in which duplicate values cannot be stored. It is an interface that implements the mathematical set. This interface contains the methods inherited from the Collection interface and adds a feature that restricts the insertion of the duplicate elements.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.011.png)








**Creating Set Objects**

Since Set is an interface, objects cannot be created of the typeset. We always need a class that extends this list in order to create an object. And also, after the introduction of Generics in Java 1.5, it is possible to restrict the type of object that can be stored in the Set. This type-safe set can be defined as:

// Obj is the type of the object to be stored in Set 

Set<Obj> set = new HashSet<Obj> ();

**Methods of Set**

|Method|`             `Description|
| :- | :- |
|add(element)  |`          `This method is used to add a specific element to the set. The function adds the element only if the specified element is not already present in the set else the function returns False if the element is already present in the Set.|
|addAll(collection)   |This method is used to append all of the elements from the mentioned collection to the existing set. The elements are added randomly without following any specific order.|
|clear()|`                `This method is used to remove all the elements from the set but not delete the set. The reference for the set still exists.|
|contains(element)|This method is used to check whether a specific element is present in the Set or not.|
|containsAll(collection)|This method is used to check whether the set contains all the elements present in the given collection or not. This method returns true if the set contains all the elements and returns false if any of the elements are missing.|
|hashCode()|`         `This method is used to get the hashCode value for this instance of the Set. It returns an integer value which is the hashCode value for this instance of the Set.|
|isEmpty()|`        `This method is used to check whether the set is empty or not.|
|iterator()|`          `This method is used to return the iterator of the set. The elements from the set are returned in a random order.|
|remove(element)|`           `This method is used to remove the given element from the set. This method returns True if the specified element is present in the Set otherwise it returns False.|
|removeAll(collection)|This method is used to remove all the elements from the collection which are present in the set. This method returns true if this set changed as a result of the call.|
|retainAll(collection)|This method is used to retain all the elements from the set which are mentioned in the given collection. This method returns true if this set changed as a result of the call.|
|size()|`                 `This method is used to get the size of the set. This returns an integer value which signifies the number of elements.|
|toArray()|`       `This method is used to form an array of the same elements as that of the Set.|

**HashSet in Java**

ava HashSet class is used to create a collection that uses a hash table for storage. It inherits the AbstractSet class and implements Set interface.

**The important points about Java HashSet class are:**

- HashSet stores the elements by using a mechanism called hashing.
- HashSet contains unique elements only.
- HashSet allows null value.
- HashSet class is non synchronized.
- HashSet doesn't maintain the insertion order. Here, elements are inserted on the basis of their hashcode.
- HashSet is the best approach for search operations.
- The initial default capacity of HashSet is 16, and the load factor is 0.75.


**Constructors of HashSet class**

To create a HashSet, we need to create an object of the HashSet class. The HashSet class consists of various constructors that allow the possible creation of the HashSet. The following are the constructors available in this class.

1\. HashSet()

This constructor is used to build an empty HashSet object in which the default initial capacity is 16 and the default load factor is 0.75. If we wish to create an empty HashSet with the name hs, then, it can be created as:

**HashSet<E> hs = new HashSet<E>();**

2\. HashSet(int initialCapacity)

This constructor is used to build an empty HashSet object in which the initialCapacity is specified at the time of object creation. Here, the default loadFactor remains 0.75.

**HashSet<E> hs = new HashSet<E>(int initialCapacity);**

3\. HashSet(int initialCapacity, float loadFactor)

This constructor is used to build an empty HashSet object in which the initialCapacity and loadFactor are specified at the time of object creation.

**HashSet<E> hs = new HashSet<E>(int initialCapacity, float loadFactor);**

4\. HashSet(Collection)

This constructor is used to build a HashSet object containing all the elements from the given collection. In short, this constructor is used when any conversion is needed from any Collection object to the HashSet object. If we wish to create a HashSet with the name hs, it can be created as:

**HashSet<E> hs = new HashSet<E>(Collection C);**





**Methods in HashSet**

|add(E e)|`          `Used to add the specified element if it is not present, if it is present then return false.|
| :- | :- |
|clear()|`                 `Used to remove all the elements from the set.|
|contains(Object o)|Used to return true if an element is present in a set.|
|remove(Object o)|`       `Used to remove the element if it is present in set.|
|iterator()|`       `Used to return an iterator over the element in the set.|
|isEmpty()|`               `Used to check whether the set is empty or not. Returns true for empty and false for a non-empty condition for set.|
|size()|`                    `Used to return the size of the set.|
|clone()                       |` `Used to create a shallow copy of the set.|


**LinkedHashSet in Java**

Java LinkedHashSet class is a Hashtable and Linked list implementation of the Set interface. It inherits the HashSet class and implements the Set interface.


![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.012.png)














**The important points about the Java LinkedHashSet class are:**

- *Java LinkedHashSet class contains unique elements only like HashSet.*
- Java LinkedHashSet class provides all optional set operations and permits null elements.
- Java LinkedHashSet class is non-synchronized.
- Java LinkedHashSet class maintains insertion order.**Constructors of LinkedHashSet Class**

**1. LinkedHashSet():** This constructor is used to create a default HashSet

LinkedHashSet<E> hs = new LinkedHashSet<E>();

**2. LinkedHashSet(Collection C):** Used in initializing the HashSet with the elements of the collection C.

LinkedHashSet<E> hs = new LinkedHashSet<E>(Collection c);

**3. LinkedHashSet(int size):** Used to initialize the size of the LinkedHashSet with the integer mentioned in the parameter.

LinkedHashSet<E> hs = new LinkedHashSet<E>(int size);

**4. LinkedHashSet(int capacity, float fillRatio):** Can be used to initialize both the capacity and the fill ratio, also called the load capacity of the LinkedHashSet with the arguments mentioned in the parameter. When the number of elements exceeds the capacity of the hash set is multiplied with the fill ratio thus expanding the capacity of the LinkedHashSet.

LinkedHashSet<E> hs = new LinkedHashSet<E>(int capacity, int fillRatio);

**SortedSet Interface in Java** 

The SortedSet interface present in java.util package extends the Set interface present in the collection framework. It is an interface that implements the mathematical set. This interface contains the methods inherited from the Set interface and adds a feature that stores all the elements in this interface to be stored in a sorted manner.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.013.png)




**TreeSet in Java**

TreeSet is one of the most important implementations of the SortedSet interface in Java that uses a Tree for storage. The ordering of the elements is maintained by a set using their natural ordering whether or not an explicit comparator is provided. This must be consistent with equals if it is to correctly implement the Set interface.

**Constructors of TreeSet Class are as follows:**

In order to create a TreeSet, we need to create an object of the TreeSet class. The TreeSet class consists of various constructors which allow the possible creation of the TreeSet. The following are the constructors available in this class:

**TreeSet():** This constructor is used to build an empty TreeSet object in which elements will get stored in default natural sorting order.

Syntax: If we wish to create an empty TreeSet with the name ts, then, it can be created as: 

TreeSet ts = new TreeSet(); 

**TreeSet(Comparator):** This constructor is used to build an empty TreeSet object in which elements will need an external specification of the sorting order.

Syntax: If we wish to create an empty TreeSet with the name ts with an external sorting phenomenon, then, it can be created as:

TreeSet ts = new TreeSet(Comparator comp); 

**TreeSet(Collection):** This constructor is used to build a TreeSet object containing all the elements from the given collection in which elements will get stored in default natural sorting order. In short, this constructor is used when any conversion is needed from any Collection object to TreeSet object.

Syntax: If we wish to create a TreeSet with the name ts, then, it can be created as follows:

TreeSet t = new TreeSet(Collection col);  

**TreeSet(SortedSet):** This constructor is used to build a TreeSet object containing all the elements from the given sortedset in which elements will get stored in default natural sorting order. In short, this constructor is used to convert the SortedSet object to the TreeSet object.

Syntax: If we wish to create a TreeSet with the name ts, then, it can be created as follows:

TreeSet t = new TreeSet(SortedSet s);

**Features of a TreeSet:**

- TreeSet implements the SortedSet interface. So, duplicate values are not allowed.
- Objects in a TreeSet are stored in a sorted and ascending order.
- TreeSet does not preserve the insertion order of elements but elements are sorted by keys.
- If we are depending on the default natural sorting order, the objects that are being inserted into the tree should be homogeneous and comparable. TreeSet does not allow the insertion of heterogeneous objects. It will throw a classCastException at Runtime if we try to add heterogeneous objects.


**Map Interface in Java**

In Java, Map Interface is present in java.util package represents a mapping between a key and a value. Java Map interface is not a subtype of the Collection interface. Therefore it behaves a bit differently from the rest of the collection types. A map contains unique keys.

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.014.jpeg)

**why and when to use Maps.**

Maps are perfect to use for key-value association mapping such as dictionaries. The maps are used to perform lookups by keys or when someone wants to retrieve and update elements by keys. Some common scenarios are as follows: 

- A map of error codes and their descriptions.
- A map of zip codes and cities.
- A map of managers and employees. Each manager (key) is associated with a list of employees (value) he manages.
- A map of classes and students. Each class (key) is associated with a list of students (value).

**Characteristics of a Map Interface**

- A Map cannot contain duplicate keys and each key can map to at most one value. Some implementations allow null key and null values like the HashMap and LinkedHashMap, but some do not like the TreeMap.
- The order of a map depends on the specific implementations. For example, TreeMap and LinkedHashMap have predictable orders, while HashMap does not.
- There are two interfaces for implementing Map in Java. They are Map and SortedMap, and three classes: HashMap, TreeMap, and LinkedHashMap.





**Method of Map:**

|Method|`             `Action Performed |
| :- | :- |
|clear()|`                 `This method is used in Java Map Interface to clear and remove all of the elements or mappings from a specified Map collection.|
|containsKey(Object)|This method is used in Map Interface in Java to check whether a particular key is being mapped into the Map or not. It takes the key element as a parameter and returns True if that element is mapped in the map.|
|containsValue(Object)|This method is used in Map Interface to check whether a particular value is being mapped by a single or more than one key in the Map. It takes the value as a parameter and returns True if that value is mapped by any of the keys in the map.|
|entrySet()|`        `This method is used in Map Interface in Java to create a set out of the same elements contained in the map. It basically returns a set view of the map or we can create a new set and store the map elements into them.|
|equals(Object)|`      `This method is used in Java Map Interface to check for equality between two maps. It verifies whether the elements of one map passed as a parameter is equal to the elements of this map or not.|
|get(Object)|`      `This method is used to retrieve or fetch the value mapped by a particular key mentioned in the parameter. It returns NULL when the map contains no such mapping for the key.|
|hashCode()|`    `This method is used in Map Interface to generate a hashCode for the given map containing keys and values.|
|isEmpty()|`     `This method is used to check if a map is having any entry for key and value pairs. If no mapping exists, then this returns true.|
|keySet()|`        `This method is used in Map Interface to return a Set view of the keys contained in this map. The set is backed by the map, so changes to the map are reflected in the set, and vice-versa.|
|put(Object, Object)|This method is used in Java Map Interface to associate the specified value with the specified key in this map.|
|putAll(Map)|`        `This method is used in Map Interface in Java to copy all of the mappings from the specified map to this map.|
|remove(Object)|`       `This method is used in Map Interface to remove the mapping for a key from this map if it is present in the map.|
|size()|`            `This method is used to return the number of key/value pairs available in the map.|
|values()|`     `This method is used in Java Map Interface to create a collection out of the values of the map. It basically returns a Collection view of the values in the HashMap.|
|getOrDefault(Object key, V defaultValue)|Returns the value to which the specified key is mapped, or defaultValue if this map contains no mapping for the key.|
|merge(K key, V value, BiFunction<? super V,? super V,? extends V> remappingFunction)|If the specified key is not already associated with a value or is associated with null, associate it with the given non-null value.|
|putIfAbsent(K key, V value)|If the specified key is not already associated with a value (or is mapped to null) associates it with the given value and returns null, else returns the current associate value.|


**Difference beween Hashtable and HashMap**

|**HashMap**|**HashTable**|
| :- | :- |
|HashMap is **non synchronized**. This means that if the hashmap is been used in a **multithread** (in two or more) environment, in that case, the hashmap can be accessed and processed in more than one thread simultaneously.|HashTable is **synchronized**, that is it makes sure that no more than one thread can access the hashtable simultaneously at a given moment of time. The thread which works on Hashtable acquires a lock on it to make the other threads wait till its work gets completed.|
|A HashMap can contain one null key and any number of null values.|A HashTable does not allow null keys and null values. If we try to store any null key or value in HashTable, it will throw a **null pointer exception** error.|
|Using the HashMap we can implement the LinkedHashMap which maintains the order of insertion, also we can implement the TreeMap which will sort the hashmap based on the ascending order of keys.|Using HashTable we cannot store the data in any kind of order. It also does not maintain the mapping in any particular order.|
|HashMap implements the Map interface, and also from the very beginning it is a part of the collection framework.|Initially HashTable was not the part of collection framework. Later on, after being reconstructed to implement the Map interface, it is been made a member of the collection framework.|
|The Iterator of HashMap is a fail-fast and it will throw an error **ConcurrentModificationException** if the map is structurally modified by adding or removing any element by any other thread. It will not throw any error if the map is modified by the iterator’s own remove() method. In simple terms, the word fail-fast |Enumerator for the Hashtable is not fail-fast. As the Hashtable is not multithread, and it can work with only one single thread at a time, so the map is not modified while running the enumerator, and it will not throw any error.|
|In the case of **HashMap** Threads are not required to wait, as multiple threads can work with **HashMap** simultaneously. So the relative performance of **HashMap** is high.|In the case of **HashTable**, it increases the waiting time of the thread as only a single thread can work with **HashTable** at a time. So the performance is low.|
|**HashMap** is introduced in the 1.2 version.|**HashTable** is introduced in the 1.0 version.|
|**HashMap** is non-legacy.|**HashTable** is a legacy.|

**Java LinkedHashMap class**

![](Aspose.Words.606d6248-36b8-4e00-b1d4-ca280a0350aa.015.png)Java LinkedHashMap class is Hashtable and Linked list implementation of the Map interface, with predictable iteration order. It inherits HashMap class and implements the Map interface.










**Points to remember**

- Java LinkedHashMap contains values based on the key.
- Java LinkedHashMap contains unique elements.
- Java LinkedHashMap may have one null key and multiple null values.
- Java LinkedHashMap is non synchronized.
- Java LinkedHashMap maintains insertion order.
- The initial default capacity of Java HashMap class is 16 with a load factor of 0.75.

**LinkedHashMap class Parameters**

Let's see the Parameters for java.util.LinkedHashMap class.

K: It is the type of keys maintained by this map.

V: It is the type of mapped values.

**Constructors of LinkedHashMap Class**

In order to create a LinkedHashMap, we need to create an object of the LinkedHashMap class. The LinkedHashMap class consists of various constructors that allow the possible creation of the ArrayList. The following are the constructors available in this class:

**1. LinkedHashMap():** This is used to construct a default LinkedHashMap constructor.

LinkedHashMap<K, V> lhm = new LinkedHashMap<K, V>();

**2. LinkedHashMap(int capacity):** It is used to initialize a particular LinkedHashMap with a specified capacity.

LinkedHashMap<K, V> lhm = new LinkedHashMap<K, V>(int capacity);

**3. LinkedHashMap(Map<? extends K,​? extends V> map):** It is used to initialize a particular LinkedHashMap with the elements of the specified map.

LinkedHashMap<K, V> lhm = new LinkedHashMap<K, V>(Map<? extends K,​? extends V> map);

**4. LinkedHashMap(int capacity, float fillRatio):** It is used to initialize both the capacity and fill ratio for a LinkedHashMap. A fillRatio also called as loadFactor is a metric that determines when to increase the size of the LinkedHashMap automatically. By default, this value is 0.75 which means that the size of the map is increased when the map is 75% full.

LinkedHashMap<K, V> lhm = new LinkedHashMap<K, V>(int capacity, float fillRatio);

**5. LinkedHashMap(int capacity, float fillRatio, boolean Order):** This constructor is also used to initialize both the capacity and fill ratio for a LinkedHashMap along with whether to follow the insertion order or not.

LinkedHashMap<K, V> lhm = new LinkedHashMap<K, V>(int capacity, float fillRatio, boolean Order);




