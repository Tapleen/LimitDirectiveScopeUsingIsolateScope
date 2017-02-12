How can you limit the scope on a directive and why would you do this? 
---------------------------------------------------------------------------------------------------

Solution:
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
By using Isolated scope of a directive. Isolated scope is a new scope created for the directive, but it will not be inherited from the parent scope which means that this scope will have no access to its outer environment. This doesn't mean that it can't access the parent scope or is totally cut off. Its just like creating a wall to stop the data penetration outside the directives. Isolate scopes do provides local scope properties to interact with parent scopes and these are :

@ one way binding which means any change made to parent scope will be available to directive scopes
= two way binding i.e any change in the parent scope will be available to directive scopes and vice a versa
& for binding methods i.e to call a functions defined in the parent controller
