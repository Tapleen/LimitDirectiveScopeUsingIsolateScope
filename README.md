How can you limit the scope on a directive and why would you do this? 
---------------------------------------------------------------------------------------------------

Solution:
----------------------------------------------------------------------------------------------------------------------------------------------------------------------
By using Isolated scope of a directive. Isolated scope as the name suggests is a new scope created for a custom directive which means it will not be inherited from the parent scope. As a result isolate scopes will have no access to its outer environment. Directives with isolate scopes comes into place when we dont have directives to interact with the parent html just like creating a wall to stop the data penetration outside the directives. However this doesn't means that it can't access the parent scope or is totally cut off from the parent HTML. Isolate scopes do interacts with parent scopes if wanted using their local scopes properties and these are :

* @ one way binding which means any change made to parent scope will be available to directive scopes
* = two way binding i.e any change in the parent scope will be available to directive scopes and vice a versa
* & for binding methods i.e to call a functions defined in the parent controller
