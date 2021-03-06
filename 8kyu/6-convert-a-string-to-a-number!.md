### Problem:
<p>Note: This kata is inspired by <a href="http://www.codewars.com/kata/convert-a-number-to-a-string/" target="_blank">Convert a Number to a String!</a>. Try that one too.</p>
<h2 id="description">Description</h2>
<p>We need a function that can transform a string into a number. What ways of achieving this do you know?</p>
<p>Note: Don&apos;t worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.</p>
<h2 id="examples">Examples</h2>
<pre><code class="language-javascript">stringToNumber(<span class="hljs-string">"1234"</span>) == <span class="hljs-number">1234</span>
stringToNumber(<span class="hljs-string">"605"</span> ) == <span class="hljs-number">605</span>
stringToNumber(<span class="hljs-string">"1405"</span>) == <span class="hljs-number">1405</span>
stringToNumber(<span class="hljs-string">"-7"</span>  ) == <span class="hljs-number">-7</span></code></pre>

### Solution

```javascript
var stringToNumber = function(str){
  return parseInt(str);
}
```

```javascript
var stringToNumber = function(str){
  return Number(str);
}
```

```javascript
var stringToNumber = function(str){
  return +str;
}
```

```javascript
var stringToNumber = function(str){
  return parseInt(str, 10);
}
```
