# Minify

A simple Java utility for minifying JSON code in your Java application.

## Reference

Minify has a simple utility method for producing minified JSON:

	/**
	 * Minifies the input JSON string.
	 * 
	 * Takes the input JSON string and deletes the characters which are insignificant to JavaScipt.  Comments will
	 * be removed, tabs will be replaced with spaces, carriage returns will be replaced with line feeds, and most
	 * spaces and line feeds will be removed.  The result will be returned.
	 * 
	 * @param json The JSON string for which to minify
	 * @return A minified, yet functionally identical, version of the input JSON string
	 */ 
	public String minify(String json)

Note: Minify also has a second utility method for producing minified JSON from a stream of input, if you'd like to work directly with streams.

## Usage

To use the library, simply instantiate an instance of the Minify class and invoke one of the minify() utility methods:

	String minifiedJson = new Minify().minify(unminifiedJson);

