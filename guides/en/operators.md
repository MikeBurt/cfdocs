# Operators in CFML

This is an incomplete / work in progress guide to operators in CFML.

### Equality

`EQ` _Script_ ✓ _Tags_ ✓

`IS` _Script_ ✓ _Tags_ ✓

`==` _Script_ ✓ _Tags_ ✖ CF8+

	if (animal == "cow") {
		return "mooo!";
	}

### Inequality

`NEQ` _Script_ ✓ _Tags_ ✓

`IS NOT` _Script_ ✓ _Tags_ ✓

`!=` _Script_ ✓ _Tags_ ✖ CF8+

	if (true != false) {
		return "sanity";
	}

### Negation

`NOT` _Script_ ✓ _Tags_ ✓

`!` _Script_ ✓ _Tags_ ✓ CF8+

	if ( !isLocalHost(cgi.remote_addr) ) {
		throw("sorry localhost only");
	}

### Comparison 



### Concatination 

`&` _Script_ ✓ _Tags_ ✓

	name = name & " Jr.";

`&=` _Script_ ✓ _Tags_ ✓ CF8+

	name &= " Jr.";	

Both code examples are equivilent.

## Compatibility Notes

The operators `==` `!=` `<` `<=` `>` `>=` do not work in tags such as cfif or cfset in Adobe ColdFusion (as of Version 11), however they work from tags on Lucee.
