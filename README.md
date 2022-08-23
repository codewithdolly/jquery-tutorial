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
    - animate- 
 - Keyboard Events: Keypress, keydown, Keyup.
 - Form Events: Submit, Change, Fucus, Blur. 
 - document/window events- load, resize, scroll, unload. 
 - 