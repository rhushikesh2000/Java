


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




