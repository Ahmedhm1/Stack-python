"""
Stack implementation in Python.

This module provides a simple Stack class that follows the LIFO 
(Last In, First Out) principle.

Features:
- Push an element onto the stack
- Pop an element from the stack
- Check if the stack is empty
- Peek at the top element
- Get the size of the stack
- String representation of the stack

Author: [Ahmed Hisham]
License: MIT
"""

class Stack:
    """
    Stack Data Structure (LIFO: Last In, First Out).

    Attributes:
        _items (list): Internal list used to store stack elements.
    """

    def __init__(self):
        """Initialize an empty stack."""
        self._items = []

    def __len__(self):
        """
        Return the number of elements in the stack.

        Returns:
            int: The current size of the stack.
        """
        return len(self._items)

    def push(self, value):
        """
        Push (add) a value onto the stack.

        Args:
            value: The element to be added.
        """
        self._items.append(value)

    def is_empty(self):
        """
        Check whether the stack is empty.

        Returns:
            bool: True if the stack is empty, False otherwise.
        """
        return len(self._items) == 0

    def pop(self):
        """
        Pop (remove) the top element from the stack.

        Raises:
            Exception: If the stack is empty.

        Returns:
            The element removed from the top of the stack.
        """
        if self.is_empty():
            raise Exception("Stack is empty")
        return self._items.pop()

    def __str__(self):
        """
        Return a string representation of the stack.

        The top of the stack is displayed at the top.
        
        Returns:
            str: Visual representation of the stack.
        """
        values = [str(item) for item in self._items]
        values.reverse()
        return "\n^\n".join(values)

    def get_top(self):
        """
        Peek at the top element without removing it.

        Raises:
            Exception: If the stack is empty.

        Returns:
            The element at the top of the stack.
        """
        if self.is_empty():
            raise Exception("Stack is empty")
        return self._items[-1]
