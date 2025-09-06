# SDE Core libraries (20250906 SDE)

## GlobalUsings
------------
create a file with the following contents in your library :

<pre>
global using g=sde.Core.Global;
global using d=System.Diagnostics.Debug;
</pre>

Then use the following statements inside your code to see what method is executing

<pre>
private void SomeCoolMethod()
{
   g.WriteLine( GetType().Name);
}

private statuc SomeCoolStaticMethod()
{
   g.WriteLine( MethodBase.GetCurrentMethod()!.DeclaringType!.Name);
}
</pre>
