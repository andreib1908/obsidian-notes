---
type: algorithm
field: computer science
field_type: stolen algortihms
main_prog_lang: java
difficulty_level: medium
main_documentation:
---
20240122101
Status: #cs
Tags: [[java]], [[algorithm]]


## Stack

You can put the length member to good use in many situations. For example, here is an improved version of the Stack class. As you might recall, the earlier versions of this class always created a ten-element stack. The following version lets you create stacks of any size. The value of stck.length is used to prevent the stack from overflowing.

```java
// Improved Stack class that uses the length array member. 

class Stack { 
	private int stck[]; 
	private int tos; 
	
	// allocate and initialize stack 
	Stack(int size) { 
		stck = new int[size]; tos = -1; 
	} 
	
	// Push an item onto the stack 
	void push(int item) { 
		if(tos==stck.length-1) // use length member
			System.out.println("Stack is full.");
		else 
			stck[++tos] = item; 
	} 
	// Pop an item from the stack 
	int pop() { 
		if(tos < 0) { 
			System.out.println("Stack underflow.");
			return 0; 
		} 
		else 
			return stck[tos--]; 
	} 
} 

class TestStack2 { 
	public static void main(String args[]) {
		Stack mystack1 = new Stack(5); 
		Stack mystack2 = new Stack(8); 
		
		// push some numbers onto the stack 
		for(int i=0; i<5; i++) mystack1.push(i);
		for(int i=0; i<8; i++) mystack2.push(i);
		 
		// pop those numbers off the stack
		System.out.println("Stack in mystack1:");
		for(int i=0; i<5; i++)
			System.out.println(mystack1.pop()); 
		
		System.out.println("Stack in mystack2:");
		for(int i=0; i<8; i++)
			System.out.println(mystack2.pop()); 
	} 
}
```

## Converting integer or long into BitSet to go through each bit individually

For longs: 

```java
public class Bits {

// Go from long to BitSet
  public static BitSet convert(long value) {
    BitSet bits = new BitSet();
    int index = 0;
    while (value != 0L) {
      if (value % 2L != 0) {
        bits.set(index);
      }
      ++index;
      value = value >>> 1;
    }
    return bits;
  }

// Go from BitSet to long
  public static long convert(BitSet bits) {
    long value = 0L;
    for (int i = 0; i < bits.length(); ++i) {
      value += bits.get(i) ? (1L << i) : 0L;
    }
    return value;
  }
}
```

For integers:

```java
/**
     * Convert an integer to BitSet.
     * @param value Value to convert.
     * @return 
     */
    public static BitSet intToBitSet(int value) {
        BitSet bits = new BitSet();
        int index = 0;
        while (value != 0) {
            if (value % 2 != 0) {
                bits.set(index);
            }
            ++index;
            value = value >>> 1;
        }

        return bits;

    }

    /**
     * Stores an integer number in a BitSet object.
     *
     * @param value integer number to store
     * @param length number of bits to use.
     * @return
     */
    public static BitSet intToBitSet(int value, int length) {
        BitSet bits = new BitSet(length);
        int index = 0;
        while (value != 0) {
            if (value % 2 != 0) {
                bits.set(index);
            }
            ++index;
            value = value >>> 1;
        }

        return bits;
    }
```

OR:

```java
int n = 12345;
BitSet bs = BitSet.valueOf(new long[]{n});
long l = bs.toLongArray()[0];
```

# References

