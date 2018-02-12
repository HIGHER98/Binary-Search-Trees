# Binary-Search-Trees

public int height(): returns the height of the tree. For this method you also need to write in comments the worst-case asymptotic running time of this method as a function of the number of keys N in the tree, and briefly explain it.

public Key median(): returns the median key in the tree.
if the tree is empty the method should return null.
If the tree has N keys K0 < K1 < K2 < ... < K(N-1), then their median is key K((N-1)/2) (here "/" is integer division). Note that the median is always a key, not the average of keys. If there is an even number of keys. For example if the keys in the tree are the A, C, U, W then the median is the key at position (4-1)/2=1, which is key C -- position numbers start at zero.

public void delete(Key key): deletes from the tree the node containing key.  
If the node to be deleted has two child nodes, then it needs to be replaced with its predecessor (not its successor). The predecessor of a key in a BST is the immediately smaller key.

public String printKeysInOrder(): returns a String containing all keys (but not the associated values) in the tree, in the order they are stored in the tree. The keys in each subtree should be contained in a parenthesis. For example when you call this method with an empty tree it should return the empty string "()". When you call it with the tree containing only a single key "A", it should return "(()A())". When you call this method on the tree in the picture below it should return the string "(((()A(()C()))E((()H(()M()))R()))S(()X()))".

public String prettyPrintKeys(): This method returns a multi-line string representation of a tree, showing only the keys in the tree. This representation should

    print the key of each node in a separate line
    print null nodes
    print the left subtree before the right subtree
    use correct indentation to print the example below.

When the method is called with an empty tree, it should return the string "-null\n".
When the method is called with the example tree shown in the picture below, it should return the string:

    -S
     |-E
    | |-A
    | | |-null
    | |  -C
    | |   |-null
    | |    -null
    |  -R
    |   |-H
    |   | |-null
    |   |  -M
    |   |   |-null
    |   |    -null
    |    -null
     -X
      |-null
      -null

Note that line breaks in a string are represented with the special sequence "\n". You should have a "\n" even after the last key in the tree.
