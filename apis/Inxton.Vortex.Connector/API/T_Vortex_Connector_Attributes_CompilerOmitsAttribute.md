# CompilerOmitsAttribute Class
 

Prevents vortex builder to create a member for specific group of output type (Shadow, Plain, Onliner).
&nbsp;<table><tr><th>![Note](media/AlertNote.png) Note</th></tr><tr><td>This attribute must be declared in the PLC code to be effective during build process.</td></tr></table>

## Examples
This example demonstrates how to prevent the vortex builder to compile specific property into specific output group. 
```
// This will not compile to 'omitsInPlainString' member into respective 'Plain' type.
{attribute clr [CompilerOmits(CompilerOmissionGroups.BuilderPlainer))]} 
ommitsInPlainString : STRING(50) := 'THIS IS OMMITED IN PLAINER';     
// This will not compile to 'ommitsInPlainAndShadowerInterfaceString' member into respective 'Plain' type and Shadow interface.
{attribute clr [CompilerOmits(CompilerOmissionGroups.BuilderPlainer, CompilerOmissionGroups.BuilderShadowerInterface))]} 
ommitsInPlainAndShadowerInterfaceString : STRING(50) := 'THIS IS OMMITED IN PLAINER';
```



## Inheritance Hierarchy
<a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">System.Object</a><br />&nbsp;&nbsp;<a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">System.Attribute</a><br />&nbsp;&nbsp;&nbsp;&nbsp;Vortex.Connector.Attributes.CompilerOmitsAttribute<br />
**Namespace:**&nbsp;<a href="N_Vortex_Connector_Attributes.md">Vortex.Connector.Attributes</a><br />**Assembly:**&nbsp;Vortex.Connector (in Vortex.Connector.dll) Version: 1.0.0+Branch.master.Sha.24c869c7af4ddc9e28426985d5ac87eee1422bb2

## Syntax

**C#**<br />
``` C#
[AttributeUsageAttribute(AttributeTargets.Property)]
public class CompilerOmitsAttribute : Attribute
```

The CompilerOmitsAttribute type exposes the following members.


## Constructors
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_Vortex_Connector_Attributes_CompilerOmitsAttribute__ctor.md">CompilerOmitsAttribute(String[])</a></td><td>
Creates an instance of CompilerOmitsAttribute.</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="M_Vortex_Connector_Attributes_CompilerOmitsAttribute__ctor_1.md">CompilerOmitsAttribute(CompilerOmissionGroups[])</a></td><td>
Creates an instance of CompilerOmitsAttribute.</td></tr></table>&nbsp;
<a href="#compileromitsattribute-class">Back to Top</a>

## Properties
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="P_Vortex_Connector_Attributes_CompilerOmitsAttribute_Omissions.md">Omissions</a></td><td>
Gets the list of groups of output type in which the member will not be included.</td></tr><tr><td>![Public property](media/pubproperty.gif "Public property")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.typeid#System_Attribute_TypeId" target="_blank">TypeId</a></td><td>
When implemented in a derived class, gets a unique identifier for this <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr></table>&nbsp;
<a href="#compileromitsattribute-class">Back to Top</a>

## Methods
&nbsp;<table><tr><th></th><th>Name</th><th>Description</th></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.equals#System_Attribute_Equals_System_Object_" target="_blank">Equals</a></td><td>
Returns a value that indicates whether this instance is equal to a specified object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.finalize#System_Object_Finalize" target="_blank">Finalize</a></td><td>
Allows an object to try to free resources and perform other cleanup operations before it is reclaimed by garbage collection.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.gethashcode#System_Attribute_GetHashCode" target="_blank">GetHashCode</a></td><td>
Returns the hash code for this instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.gettype#System_Object_GetType" target="_blank">GetType</a></td><td>
Gets the <a href="https://docs.microsoft.com/dotnet/api/system.type" target="_blank">Type</a> of the current instance.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.isdefaultattribute#System_Attribute_IsDefaultAttribute" target="_blank">IsDefaultAttribute</a></td><td>
When overridden in a derived class, indicates whether the value of this instance is the default value for the derived class.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.attribute.match#System_Attribute_Match_System_Object_" target="_blank">Match</a></td><td>
When overridden in a derived class, returns a value that indicates whether this instance equals a specified object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.attribute" target="_blank">Attribute</a>.)</td></tr><tr><td>![Protected method](media/protmethod.gif "Protected method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.memberwiseclone#System_Object_MemberwiseClone" target="_blank">MemberwiseClone</a></td><td>
Creates a shallow copy of the current <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr><tr><td>![Public method](media/pubmethod.gif "Public method")</td><td><a href="https://docs.microsoft.com/dotnet/api/system.object.tostring#System_Object_ToString" target="_blank">ToString</a></td><td>
Returns a string that represents the current object.
 (Inherited from <a href="https://docs.microsoft.com/dotnet/api/system.object" target="_blank">Object</a>.)</td></tr></table>&nbsp;
<a href="#compileromitsattribute-class">Back to Top</a>

## See Also


#### Reference
<a href="N_Vortex_Connector_Attributes.md">Vortex.Connector.Attributes Namespace</a><br />