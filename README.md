# simple-multi-lang.js
A Simple Search Engine Friendly Multi-language plugin for jQuery.

## How to use
All translations are wrapped in HTML tags like this:

	<div>
		<span lang="en">Hello world!</span>
		<span lang="fr">Bonjour le monde!</span>
		<span lang="cn">你好，世界！</span>
	</div>

Language can be switched like this:

	$('span[lang]').languageSwitcher('en');

Don't forget to hide other language:

	<style>
		span[lang="fr"] {display: none}
		span[lang="cn"] {display: none}
	</style>

## Online demo
https://jsfiddle.net/zhangchengx/xpvt214o/470356/

## Example
### Button:

	<button onclick="$('span[lang]').languageSwitcher('en')">English</button>
	<button onclick="$('span[lang]').languageSwitcher('fr')">French</button>
	<button onclick="$('span[lang]').languageSwitcher('cn')">Chinese</button>
	
### A

	<a href="#" onclick="$('span[lang]').languageSwitcher('en')">English</a> 
	<a href="#" onclick="$('span[lang]').languageSwitcher('fr')">French</a> 
	<a href="#" onclick="$('span[lang]').languageSwitcher('cn')">Chinese</a> 

### Radio:

	<script>
	$("input[type=radio]").change(function() {
		$("span[lang]").languageSwitcher( $(this).attr("id") );
	});
	</script>
	<input type="radio" id="en" name="lang" checked><label for="en">English</label>
	<input type="radio" id="fr" name="lang"><label for="fr">French</label>
	<input type="radio" id="cn" name="lang"><label for="cn">Chinese</label>

## Todo

...
