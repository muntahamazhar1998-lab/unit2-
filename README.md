# unit2-
Unit 2 Discussion: Stacks and Queues


---

#  **ImInitial Discussion Post – Unit 2: Stacks and Queues**



For this unit, I implemented both a **Stack (LIFO)** and a **Queue (FIFO)** in Python by completing all the TODO prompts in the starter file. My stack uses a Python list, which makes push and pop operations straightforward because both happen at the same end. For the queue, I used `collections.deque` since it allows efficient additions at the back and removals from the front without slowing down as the structure grows.

### **Design Approach & Application Scenario**  
To demonstrate how these structures work in real life, I chose two scenarios that clearly show the difference between LIFO and FIFO behavior.  
- My **stack** models an undo system in a text editor. The most recent action—like typing or deleting is always undone first, which perfectly matches LIFO behavior.  
- My **queue** models customers waiting in line at a coffee shop. The first customer to arrive is the first one served, which reflects FIFO processing.

### **Why Stack = LIFO & Queue = FIFO**  
A stack follows **Last‑In, First‑Out** because items are added and removed from the same end. The newest item must be accessed first, just like undoing your most recent change.  
A queue follows **First‑In, First‑Out** because items enter at the back and leave from the front. This keeps the order fair and predictable, like a line of customers or a printer job queue.

### **Memory Growth**  
Both data structures grow **linearly (O(n))** as more items are added. Each new element requires additional memory, so the total space increases proportionally with the number of stored items. Removing items decreases memory usage accordingly.

### **Reflection**
Completing this assignment helped me understand stacks and queues on a deeper, more practical level. I’ve used undo buttons and waited in lines many times, but actually implementing LIFO and FIFO behavior in Python made those concepts feel much more concrete. Writing the stack and queue operations myself showed me how important structural rules are, especially when you’re managing data that needs to stay predictable and organized.

One challenge I ran into was making sure my operations handled empty structures correctly. At first, I didn’t think much about edge cases, but testing my code made it clear how easily a pop or dequeue can cause errors if the structure is empty. Adding defensive checks helped me avoid crashes and made my program more reliable. I also learned how important it is to read error messages carefully—they really do point you in the right direction.

This assignment also made me think more about how these structures show up in real applications. Stacks work perfectly for undo systems or browser history because the most recent action needs to be reversed first. Queues make sense for things like customer service tickets or print jobs, where fairness and order matter. Overall, building these structures myself helped me appreciate how much they shape the way software behaves.
