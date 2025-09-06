# SDE Core libraries (20250906 SDE)

## GlobalUsings
------------
create a file with the following contents in your library :

<pre>
global using g=sde.Core.Global;
global using d=System.Diagnostics.Debug;
</pre>

Then use the following statements

<pre>
g.WriteLine( GetType().Name);
g.WriteLine( MethodBase.GetCurrentMethod().DeclaringType.Name); 	// -- static
g.WriteLine( MethodBase.GetCurrentMethod()!.DeclaringType!.Name);	// --- Dereference of a possibly null reference
</pre>
