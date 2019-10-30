<h1>Page 3 </h1>
<p> 
  <a href="index.html">Home</a> <br> 
  <a href="page2.html">Page 2</a>
  <a href="Idioms.html">Idioms</a>
</p>

<h2>Here is a list of all names with random(ish) verb + adverb</h2>

<button onclick="makeSentence()">Click me</button>

<p id="demo"></p>

<script>
function makeSentence() {
var person = {
    names: [ "Brian","Betty","Fiona", "Freddy", "Mini", "Marvin", "Alice", "Bob", "Jane", "Arthur", "Vincent", "Amy", "He", "She" ],
    verbs: [ "speaks", "eats", "runs", "walks", "drinks" ],
    adverbs: ["slowly", "quickly", "nicely", "noisily", "a lot", "a little", "rarely" ]
    };
    
 var i
 var text ="";
 for (i=0; i <person.names.length; i++) {
    name = person.names[Math.floor(Math.random() * person.names.length)];
    verb = person.verbs[Math.floor(Math.random() * person.verbs.length)];
    adv = person.adverbs[Math.floor(Math.random() * person.adverbs.length)];
    
    text += name + " " + verb + " " + adv + "<br>";
    
    document.getElementById("demo").innerHTML = text; 
  }

}
</script>

