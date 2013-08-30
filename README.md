<h1>Color.js</h1>
<h2>abstract Color management class written in JavaScript</h2>
<p><a href="http://moagrius.github.io/Color/Color.html" target="_blank">Documentation</a></p>
<p>This class allows a Color to be created in any format (RGB, hex, decimal, HSL, HSV, CSS, etc), while allowing any component to be manipulated.</p>
<ul>
<li>new Color();	</li>
<li>new Color('#FF9900');	</li>
<li>new Color(element.style.color);	</li>
<li>new Color('pink');	</li>
<li>new Color(123456);	</li>
<li>new Color({ red : 255, green : 100, blue : 0 });	</li>
<li>new Color(colorInstance);</li>
</ul>
<p>For example, you can create a color in RGB format, but then modify the lightness, or brightness, or saturation - it need not be converted between formats (although format output is also available).</p>
<p>Component methods include:<p>
<ul>
<li>.red()	</li>
<li>.green()	</li>
<li>.blue()	</li>
<li>.hue()	</li>
<li>.saturation()	</li>
<li>.lightness()	</li>
<li>.brightness()	</li>
<li>.hex()	</li>
<li>.decimal()</li>
</ul>
<p>Component methods signatures are similar to jquery mutators - invoked without arguments, the method functions as a getter, and returns the current value;
invoked with an argument, they function as setters, and update that value on the calling instance.</p>
<pre>// usage...
var color = new Color('#FF9900');
color.brightness(20);
element.style.backgroundColor = color;
console.log(color.getRGB());
console.log(color.saturation());</pre>