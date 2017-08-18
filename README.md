# vanilla-modal
A material design-esque modal that uses no libraries, only HTML, CSS and JS.

Include ```modal.css``` at the top of your html file, and ```modal.js``` at the bottom of your html file.

```<link rel="stylesheet" type="text/css" href="modal.css">```
```<script src="modal.js"></script>```

First put the html code below somewhere in your body, anything outside of this div will be covered
by a black overlay and rendered unusable (apart from the modal) when the modal is toggled on.

```<div id="modal-overlay" class="modal-overlay"></div>```

Next, put this html code somewhere in your body, it will add the modal in a hidden state to your page.
The modal will be centered via "margin: 0 auto;" but this can be changed in the css.

```
<div id="modal-box" class="modal-box">
    <div class="modal-header">
        <div class="modal-close-btn">
            <button id="close-modal" onclick="toggleModal()">Close</button>
        </div>
        <div class="modal-title">
            <h4>Modal Title</h4>
        </div>
    </div>
    <div class="modal-content">
    </div>
</div>
```

To open or close the modal, call the function 'toggleModal()'.

Hopefully this is useful to someone, it doesn't depend on any libraries and so I thought I should share it as it is easy to add to a web page. If you wish to change the code and make it better, by all means create a pull request.

![Modal With Content](http://imgur.com/7z5JbhZ)

![Modal Without Content](http://imgur.com/UtO8N92)

