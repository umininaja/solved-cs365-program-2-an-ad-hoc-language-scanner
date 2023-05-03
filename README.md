Download Link: https://assignmentchef.com/product/solved-cs365-program-2-an-ad-hoc-language-scanner
<br>
<strong>Objective </strong>

Learn the basics of programming an ad-hoc language scanner

<strong>Assignment </strong>

Build the start of an ad hoc scanner to handle a simple language. The output for the scanner will be a list, and in order, of the type of token, a comma, and the actual value of the token (the token and the lexeme).




<ul>

 <li>This must be written in Java.</li>

 <li>If you create more than one Java file, compress all of your files into a single file for uploading.</li>

 <li>You must use file input. Pick up the source code file name from the command line. Exit <strong>gracefully</strong> with an error message if the input file does not exist.</li>

 <li>Write the output to the screen.</li>

 <li>There is no error checking required of file names OTHER than to ensure if they are present – your program will not be given an illegal file name when testing.</li>

 <li>There is no guarantee of whitespace except <em>where required</em> to separate tokens. A line feed is a form of whitespace. There will not be any tab characters in the source code.</li>

 <li>An &lt;id&gt; token is a string of alphabetic characters starting with an upper or lower case ‘a’-‘z’, followed by either an upper or lower case ‘a’-‘z’ or ‘0’-‘9’ (standard identifier rules without the underscore character). An &lt;id&gt; cannot be one of the reserve words in the grammar.</li>

 <li>A &lt;number&gt; can be either an integer or a floating point value. A floating point value WILL have at least one digit both in front and after a decimal point.</li>

 <li>A &lt;rel_op&gt; token is either a &lt;, &gt;, &lt;=, &gt;=, ==, or !=</li>

 <li>The &lt;assign&gt; token, the assignment operator, is the equal sign (“=”).</li>

 <li>The “reserved” words in the grammar are all lowercase and casespecific. They include: input, print, begin, end, if, and Their respective tokens are &lt;input&gt;, &lt;print, &lt;begin&gt;, &lt;end&gt;, &lt;if&gt;, and &lt;else&gt;.</li>

 <li>A # symbol indicates a comment. Ignore the remainder of the current physical line. This will not generate a token.</li>

 <li>If your program encounters text that is not a valid token, write out an</li>

</ul>

&lt;error&gt; token and the invalid text (not the remainder of the file). Stop processing the input file after dealing with an error.

<h1>For example, if the input file contains:</h1>

#sample “source code” for simple language min = 0 input a input b if a &lt; b begin    min = a end else    min = b

print min




your output should contain:

&lt;id&gt;, min

&lt;assign&gt;, =

&lt;number&gt;, 0

<h1>&lt;input&gt;, input</h1>

&lt;id&gt;, a

&lt;input&gt;, input

&lt;if&gt;, if

&lt;id&gt;, a

&lt;rel_op&gt;, &lt;

&lt;id&gt;, b

&lt;begin&gt;, begin

&lt;id&gt;, min

<h2>&lt;assign&gt;, =</h2>

&lt;id&gt;, a

&lt;end&gt;, end

&lt;else&gt;, else

&lt;id&gt;, min

&lt;assign&gt;, =

&lt;id&gt;, b

&lt;print&gt;, print

&lt;id&gt;, min