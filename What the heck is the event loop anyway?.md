- Javascript's runtime is *single-threaded* (can only run one piece of code at a time), but thanks to the browser APIs, it can do multiple things at the same time
- Javascript must be asynchronous, because otherwise you'd just have to wait for a process to finish, while the browser would be stuck
- The asynchronous model looks like this:
	1. Function is pushed to *function stack* -> it either returns something, or 
	2. It calls some *webapi function*  (like starting a timer), which will handle the process, therefore we can remove the function from the stack, and the rest of the functions on the stack can continue being executed. 
	3. The specific webapi pushes the function to a *task queue* (it can't just push it to the stack, because some process might be already executing,  so functions would be called randomly. Instead, it needs to wait for the stack to empty). 
	4. Now it's *event loop*'s job to push it back onto the stack: *the event loop checks if the stack is empty. If it is empty, it pushes the first function of the task queue onto the function stack*.
- A *callback* is some function that will be called by the event loop sometime