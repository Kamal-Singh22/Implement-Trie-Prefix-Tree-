# Implement-Trie-Prefix-Tree-
Design and implement a Trie (Prefix Tree) data structure that supports the following operations:  insert(word): Inserts the string word into the trie. search(word): Returns true if the string word is in the trie (i.e., was inserted before), and false otherwise. startsWith(prefix):
Explanation:
TrieNode Class:

Each node contains an array children of size 26 (for each lowercase letter) and a boolean flag isEndOfWord to indicate if a node corresponds to the end of a word.
insert(String word):

Traverse the Trie according to each character of word.
Create new nodes when necessary.
Mark the end node with isEndOfWord = true.
search(String word):

Use the helper method searchPrefix to traverse the Trie.
Return true if the node is found and is marked as an end-of-word.
startsWith(String prefix):

Similar to search but only checks for the existence of the prefix in the Trie.
