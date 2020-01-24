# AgletJS

[New Version!](https://github.com/lemmin/agletjs2)



AgletJS aims to fix the disconnect between the DOM and JS. Aglets work similarly to jQuery objects, but with very few extra features. The main purpose of an Aglet is to provide a more concise, hierarchical structure for your application's variable references to DOM objects.


### For example, with the following code:
<pre>
	<form <b>ag-name="search"</b>>
		<label>
			Search:
			<input <b>ag-name="terms"</b> type="text"/>
		</label>
		<div <b>ag-name="options"</b>>
			<label>
				<input <b>ag-name="exact"</b> type="checkbox"/>
				Match Exact Phrase
			</label>
			<label>
				<input <b>ag-name="regex"</b> type="checkbox"/>
				Use Regular Expression
			</label>
		</div>
	</form>
</pre>

Your application will automatically have access to variables like `search.terms` and `search.options.exact`


Aglets can also be defined as components to be added to the DOM at any time. 
