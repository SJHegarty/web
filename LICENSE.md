The really fucking dumb license agreement.
You can add to this license, you cannot remove from this license.

This license is completely unenforcable.
This license offers no guarantees what-so-ever.
This license reserves the right to be incoherant.

The term "Content" 
	shall be used to refer to any and all project elements stored locally or in version-control, 
	excluding Meta-Elements as required for the purposes of access to and execution of version-control services and protocols.

the term "End-User" refers to who the fuck ever has access to this license and the Content licensed here-[in, under 
The term "Modified-Content" shall be used to refer to any and all 
No Content containted 
All Con
The term "Code" shall be used to refer any and all descriptive content within the licensed content

You are prohibitted from viewing or compiling
Use, modification, viewing and distribution of an

Element e;
$cns Meta-Element cme = $meta(e); 	//create a Meta-Element for the value of e at this moment
$dyn Meta-Element dme = $meta(e);	//create a Meta-Element for the value of e at what-ever moment dme happens to be used.


//This is also nice for string twiddling:
$cns String foo = ~"@$meta(blah).name; = @blah ~: String;";
$dyn String bar = ~"@$meta(blah).name; = @blah ~: String;";

//Dynamic values cannot be used as keys.
[(String key) -> (Value val)] map = TreeMap<~>.new();

map[foo] = some-val; //Oooh, go on then.
map[bar] = some-other-val; //Or maybe, go fuck yourself.
map[$const(bar)] = yet-another-val; // there we go.

$ex ?<T> <:() -> ():> {	
	//an executable, of Mystery-Type T,
	//<: .... :> parameters and return type.
	//() no args, no return type. Why the generics?
	
	Element e;
	$cns $Meta-Element cme = $.meta(e); 	//create a 
	$dyn $Meta-Element dme = $.meta(e);
	

}
	
A stream should beging with a start of stream token, all machines should be made to create a transition from the initial state to the initial state on the start of stream token.
	
Since the token only appears once this is not an invalid thing to do.
I don't care if anyone's injecting random start of streams.

That allows a line header to be detected even at the start of the file.

A Tree structure should have some function that returns a set of Paths.
I should then 

$[cns type] Whaver ?<E ~ Const> {
}
	
$dyn Whaver<T> w = some-whaver;	//No
$cns Whaver<T> w = some-whaver;	//Sure
Whaver<T> w = some-whaver;	//As above.

$dyn ?Whaver<?T> whaver-builder = some-whahver ~: Dynamic;

//{
	Now we're crawling into the roots.
	We don't have a Whaver, we have something that is shaped like a Whaver, but is subject to change and mutation.
	We can do whatever we want, then cast it back
}
...//Mutate the builder.

Whaver<T> robo-whaver = whaver-builder ~: Const;
//{
	This thing still should have the data structure of a Whaver (unless you've done something weird); it's more likely that the data itself is invalid
	the conversion process will need to validate.

	The ?X Meta-Type is recursive, and singularly applicative.
	$[cns type] ?<X ~ [Supertype-A<E, X>, Supertype-B<C>]> Q<X>::;
	?X == ??X
	?X<T> == ?X<?T>
	X<?T> != ?X<?T>
	
	$Auto unused = .$meta(some-value);	
	//'$'[A...Z]*<1+>[a...z] system class
	//'.$'*<1+>[a...z] system funct

	X<T> value = ...;
	X<?T> builder = value;	//auto-cast in the case of obvious intent, this initialises the builder to the value of the constant.
	.mutate(builder);
	
	//Casts descend recursively through the structure converting all dynamic elements and validating.
	
	//This can throw an exception and returns a compiler warning
	X<T> processed = builder;
 	
	//This cannot throw an exception
	X<T>? processed = builder;
	$.if(processed){
		...//No error, conversion valid
		
		...//Do the things
	}..
	$.else{	
		//{
			There is no .else system method, parallel compilation fails to find a handler
			However, the $.if block, having detected that it is continued, processes the block instead.

			In the event that there was a $.else method defined in the universal context (and not just that of continuations),
			The parallel compiler should attempt to process the code as a independant block
			However, even in the result of successful compilation, the result will be disgarded as the continuation context takes precedence.
		}
		//Just because an object does not have a value, does not mean that meta information about it does not exist
		$Auto meta = $Meta-X<T>.new(processed);
		//Cast the cause for non-existence (the point of the failure to convert) to an error and throw it.
		$.throw(meta.why ~: Error);
	}
	

}


$type Tree ?<E ~ Const>{
	$cns Node<E> root;
	//figure out what syntax should be used for the pathfinder function.
}
$type 
	
$type Eventually ?<T> ~ Task{
	$[undefined do] <:() -> (T? value):>;
	$[undefined on-done] ?<T> <: (T value) -> () :> ;
	$[undefined on-done] <: () -> () :> ;
}
	
$type Map ?<E ~ <:Key ~ Const, Val ~ Const:>> ~ Tree<E> {
	
}
