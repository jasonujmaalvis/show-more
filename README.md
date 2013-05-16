<h1>Show More</h1>

Author: Jason Alvis<br />
Author Email: alvis.jason@gmail.com<br />
Version: 1.0<br />
License: http://opensource.org/licenses/afl-3.0.php  Academic Free License (AFL 3.0)<br />

<h2>Brief</h2>
A neat little plugin that allows you to show / hide content (toggle) on clicking a trigger. Useful for areas of a website with restricted space but you still want to show a lot of content. Typically used on text blocks where you reveal a small portion of the text and show more on clicking a trigger.

Very easy to implement please follow the instructions below:

<h3>HTML</h3>


<div class="showmore">
     <h2>Show more block</h2>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. In et felis rutrum neque aliquam hendrerit eu et massa. Phasellus fermentum, elit nec vulputate vehicula, massa lorem ultrices purus, id pulvinar elit massa et ligula. Suspendisse vulputate quam non sem iaculis auctor. Maecenas ut nisi ut urna bibendum aliquet non vestibulum mi. Fusce euismod condimentum sem, vitae elementum dui mattis eget. Duis imperdiet congue justo, eget commodo risus imperdiet sit amet. Aenean sem augue, pulvinar nec sagittis eu, hendrerit vitae sapien. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse laoreet, diam sed faucibus ultricies, velit tortor fringilla ligula, sed malesuada magna justo nec ligula. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Etiam metus leo, tincidunt eu fringilla at, tincidunt et leo. Aliquam nec eros eu nisl consectetur mattis. Nullam eleifend velit at est varius non sagittis ligula tincidunt. Aenean elementum rhoncus mattis.</p>	
     <p>Maecenas ullamcorper erat ut leo imperdiet sed aliquet nunc congue. Maecenas consectetur purus ac lorem pellentesque dignissim. Nunc aliquet sapien sit amet odio tincidunt a commodo ante dignissim. Praesent vel ligula odio, sit amet fringilla tortor. Ut nec erat sit amet nisl varius euismod a ut lorem. Morbi dapibus dui luctus lorem fermentum at gravida sapien auctor. Aliquam erat volutpat. Aenean turpis metus, laoreet sit amet venenatis quis, ornare vitae erat. Integer gravida aliquam fringilla. Curabitur eros eros, placerat non pharetra id, fringilla vitae justo. Aenean sagittis facilisis sapien, eu varius augue adipiscing ut.</p>	
</div>


<h3>jQuery</h3>

Add the following code to your JavaScript file typically on a document.ready:
       
$('.showmore').showMore({
     speedDown: 300,
     speedUp: 300,
     height: '165px',
     showText: 'Show more',
     hideText: 'Show less'
});

<h3>Minimum CSS styles</h3>

To ensure consistency across multiple browsers please ensure the showmore block has a line-height specified. This will then provide a accurate height and display correctly.

.showmore { line-height:18px; }
.showmore_content { position:relative; overflow:hidden; }			
.showmore_trigger { width:100%; height:45px; line-height:45px; cursor:pointer; }
.showmore_trigger span { display:block; }
