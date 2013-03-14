# jquery-confirm

Create native confirmation dialog boxes based on data attributes.

## Demo
http://jsfiddle.net/joshmoody/TbY8r/

## How it works
1. Give your element (button, input, anchor, etc) a data attribute named data-confirm containing the confirmation text you want displayed on click.

2. On load, add the confirm method to some selector(s) for your confirmation elements.

3. When the element is clicked, the browser's native confirmation prompt will display with the text from the data-confirm attribute.  Canceling will do nothing, Confirming will allow the default action to occur (like a form submit).

## Example
```javascript
	<script src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
	<script src="//path/to/jquery.confirm.js"></script>
	
	<input type="submit" id="confirm-button" class="confirm"
        data-confirm="Are you sure you want to delete the internet?  This action cannot be undone. Proceed?"
        value="Delete The Internet" />
        
	$(function() {
 		$('.confirm ').confirm();
	});
		
```

## TO DO
- [ ] Generate minified version. Yeah, it's tiny, but every bit helps.
