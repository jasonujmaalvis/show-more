<h1>Show More</h1>

Author: Jason Alvis<br />
Author Email: alvis.jason@gmail.com<br />
Version: 1.0<br />
License: http://opensource.org/licenses/afl-3.0.php  Academic Free License (AFL 3.0)<br />

<h2>Brief</h2>
A neat little plugin that allows you to show / hide content (toggle) on clicking a trigger. Useful for areas of a website with restricted space but you still want to show a lot of content. Typically used on text blocks where you reveal a small portion of the text and show more on clicking a trigger.

Very easy to implement please follow the instructions below:

<h3>jQuery</h3>

(function($) {
  $(document).ready(function() {
       
    $('.showmore').showMore({
      speedDown: 300,
      speedUp: 300,
      height: '165px',
      showText: 'Show more',
      hideText: 'Show less'
    });
	      
  });
})(jQuery);

<h3>Minimum CSS styles</h3>
.showmore_content { position:relative; overflow:hidden; }			
.showmore_trigger { width:100%; height:45px; line-height:45px; cursor:pointer; }
.showmore_trigger span { display:block; }
