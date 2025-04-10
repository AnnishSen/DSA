# ❓ Doubt: Why do we write `ListNode*` or `TreeNode*`?

## 🔹 What does `*` mean in C++?

- The `*` symbol is called the **pointer declarator** or **dereference operator**.
- Writing `ListNode* ptr;` means `ptr` is a **pointer to a ListNode object**.

## 🔹 Why use `*` for linked lists and trees?

- Because these data structures are **dynamic**.
- Each node (`ListNode`, `TreeNode`) points to other nodes.
- Using pointers allows us to:
  - Dynamically allocate memory (`new`)
  - Pass and return references to nodes efficiently

## 🔹 Example

```cpp
struct ListNode {
    int val;
    ListNode* next; // next is also a pointer
};

ListNode* head = new ListNode(5); // head is a pointer to a new node

