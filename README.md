# Binary Trees

C project implementing basic operations on binary trees.

## Features

- Node creation and insertion (left / right)
- Tree traversals (preorder, inorder, postorder)
- Height and balance factor calculation
- Full, perfect and complete tree checks
- Sibling and uncle node lookup
- Tree deletion

## Example

```c
binary_tree_t *root;

root = binary_tree_node(NULL, 98);
root->left = binary_tree_node(root, 12);
root->right = binary_tree_node(root, 128);
root->left->left = binary_tree_node(root->left, 10);
root->left->right = binary_tree_node(root->left, 54);

      (98)
     /    \
   (12)  (128)
   /  \
 (10) (54)

Compilation:
gcc -Wall -Wextra -Werror -pedantic -std=gnu89 *.c -o bt
