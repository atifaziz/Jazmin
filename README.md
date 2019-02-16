# Jazmin, the JavaScript Source-Compressor

Jazmin is a console-based utility and an MSBuild task that filters JavaScript
by removing comments and unnecessary whitespace. It typically reduces the size
of the script by half, resulting in faster downloads. It also encourages a
more expressive programming style because it eliminates the download cost of
clean, literate self-documentation. Jazmin _does not_ modify the behavior of
the original JavaScript source in any way.

Jazmin is a straight C# port of [JavaScript Minifier][jsmin] that was
originally written by [Douglas Crockford][crockford] in C. Jazmin behaves
identically to JSMin so [all the documentation on JSMin][jsmin] also applies
to Jazmin.

[jsmin]: http://www.crockford.com/javascript/jsmin.html
[crockford]: http://www.crockford.com/


## Usage

The command-line version of Jazmin reads the source from the standard input
and produces the compressed version on the standard output. To compress a
single file, pipe through Jazmin like this on your shell prompt:

    $ jazmin < some.js > comp/some.js

## License

Jazmin is distributed under the [OSI]-approved and liberal [BSD License][lic]:

Copyright &copy; 2005, Atif Aziz. All rights reserved. Portion Copyright
&copy; 2001 Douglas Crockford

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

- Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.
- Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.
- Neither the name of the author nor the names of its contributors may be used
  to endorse or promote products derived from this software without specific
  prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

[OSI]: http://www.opensource.org/
[lic]: http://opensource.org/licenses/bsd-license.php
