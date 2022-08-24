# jquery-tutorial-

# There are multiple ways to use Jquery
    1. you can download it and import that and use.
        - Now in download also there are 2 types "Download the compressed" and "Download the uncompressed,"
            -Compressed is used in production level. (prefer this)
            -uncompressed you can see the whole code that how it has written.
    2. import the version and start using it.
        - this methid called "jquery CDN(Content delivery network). it will surve the jquery from cdn itself. 
    3. install it and use it.
        - you can install it will "npm i" and use it.

# jquery syntex
    - it start with $. (this "$" means "jquery". if you write "jquery" at "$" place then also it will work.)
    - $('selector').action();
    -$('selector').hide();
    -$('button').click(function(){
        log('you clicked btn.')
        $(this).hide();//that particular thing only hide.
    }); //do this when btn click.
        - this keyword - Suppose you have multiple button you have targeted with tag only. So if you click then all button will hide. so to solve this issue we use this.hide.
        - 'button' is just a selector. you can select this by .class and #ID as well.


# Before loding HTML jquery load and work, So for that we use

                1.     $(document).ready(function () {
                        $("p").click(function () {
                        alert("Hey P");
                        });});

                                || OR ||

                2.      $(function () {
                        $("p").click(function () {
                            alert("Hey P");
                        });});
                (So you can direact write only $ and remove "(document).ready". but good practice is First method only.)

# Selectors:-
    - Element/Tags
    - ID
    - Class
    - * (Universal selectors)
    - $(p.odd).click(); (p is element)- It will select odd.
    - $(p:first).click(); - It will select first para will be clicked.
    - 



# Events in jquery
 - Mouse Event: click, dblclick, mouseenter, mouseover, mousemove, mouseleave, mousedown, mouseup.
    - click- on click, show&Hide,toggle button,  fadeIn(), fadeOut(), fadeToggle(), fadeTo(), slideUp and slideDown with SlideToggle
 - Keyboard Events: Keypress, keydown, Keyup.
 - Form Events: Submit, Change, Fucus, Blur. 
 - document/window events- load, resize, scroll, unload. 
 - 

# To get the value 
    - to get text/elemet value we use .text or .html. but
    - to get form, input or textarea value we use .val (to teplace text also we use val only NOT "text or html- these are only of text and element.")

# empty vs remove value 
    - $('#wiki').empty(); - this will empty the value of element.
    - $('#wiki').remove(); - This will delete the Element from DOM.

# add/remove class and ID
    - $('#wiki').addClass('myClass'); 
    - $('#wiki').removeClass('myClass'); 
    - $('#wiki').toggleClass('myClass'); 
      
# add CSS
    -$("#rana").css('color', 'red'); //set css value
    -$("#rana").css('color'); //findout the css value 

# what is Ajax?
    - Ajex is an art of exchanging data without loading a page. 

# What is CORS error?
    - Sometimes Google doesnot allow you to use data from other origin and that error is called CORS error.

# AJAX Using jQuery
    - GET METHOD:- 
        - $.get('https://code.jquery.com/jquery-3.3.1.js', function (data, status) { alert(data); })
        - $.get('https://code.jquery.com/jquery-3.3.1.js', function (data, status) { alert(status); })

    - POST METHOD
         $.post('https://code.jquery.com/jquery-3.3.1.js',
           { name: 'harry', channel: 'code with harry' },
             function (data, status) { alert(status) });
