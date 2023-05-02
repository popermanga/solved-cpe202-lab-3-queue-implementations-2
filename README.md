Download Link: https://assignmentchef.com/product/solved-cpe202-lab-3-queue-implementations-2
<br>
<strong>Queue Implementations Goals: </strong>

<ul>

 <li><strong>Implement a Queue class using a link-based data structure: queue_linked.py </strong></li>

 <li><strong>Implement a Queue class using a circular array: queue_array.py </strong></li>

</ul>

Before doing this lab make sure to read over section 3.10, 3.11, and 3.12 carefully. You will not be doing the implementation described in section 3.12, but it will help you understand the underlying concepts.

<ul>

 <li>In the first implementation, you will use a linked structure similar to the linked structure used in implementing the Stack ADT (i.e. create a Node class). In this case, there must be a way to add items to the rear of the list and remove items from the front of the list, as illustrated below.</li>

 <li>The second implementation will use a circular array for storing the items in the queue. There are different ways of doing this, but they share the idea presented in the picture below.  Items are added to the rear of the queue using the next “free entry” in an array. Items are removed from the front of the queue.  The indices front and rear are incremented as items are added and deleted from the queue, and the indices “wrap around” when they reach the end of the array.  Why is using a circular array better than what the text does (i.e. inserting new items at index 0 of array, and removing items from the end of the array)?</li>

</ul>

For both Queue implementations:

<ul>

 <li>Attempting to enqueue an item into a full Queue will raise an IndexError</li>

 <li>Attempting to dequeue an item from an empty Queue will raise an IndexError</li>

 <li>All methods must have <strong><em>O(1)</em></strong> performance (the speed must not be affected by the size of the queue)</li>

 <li>As with your stack implementations, you <strong>may NOT use</strong> any of the following Python List operations:

  <ul>

   <li>append() o insert() o extend() o remove()</li>

   <li>pop()</li>

   <li>+ (concatenations)</li>

  </ul></li>

</ul>

The following starter files are available on GitHub.  Complete the implementations and ensure that your implementations are committed and pushed to GitHub.

<ul>

 <li><strong>py</strong>: Contains an array (Python List) based implementation of the <strong>Queue</strong> class</li>

 <li><strong>py</strong>: Contains a linked based implementation of the <strong>Queue</strong> class</li>

 <li><strong>py:</strong> Contains your set of thorough tests to ensure your implementations work correctly.</li>

</ul>

(Note that the class in each stack implementation is named <strong>Queue</strong>, and both implementations must follow the same specification. This allows one set of tests in <strong>queue_tests.py</strong> that can be used for both implementations by just changing which file is used when importing