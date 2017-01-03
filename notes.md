## Notes

1. Things are already working and looking as they should. Header bar is displaying and pulling to right of screen.

Simply with the use of classes.

```html
<div class="container">
  <header class="page-header">
    <ul class="nav nav-pills pull-right">
      <li><a href="#">Home</a></li>
      <li><a href="#">About Ribbit</a></li>
      <li><a href="#">Treehouse</a></li>
    </ul>

    ...
  <div>
```

2. Lesson learned Gill mentioned use of bootstrap themes & promised to link to them in notes.
Finally, paused video and entered the path displayed [here](http://getbootstrap.com/examples/theme/#).

I noticed that documentation page used the following notation to distinguish via notes indicating when things would end. Just a standard way to distinguish b/n parts is beautiful! Esp. using tag end notation. Like </patriarchy>

```html
 </div><!-- /.col-sm-4 -->
 ... lots of things b/n.
</div><!-- /.col-sm-4 -->
```

3. Question: what's the convention of naming class order?

```html
<p class="btn-group">
  <!-- do you want to keep the size of the button first? and plain btn class to go second? -->
  <a class="btn-lg btn btn-success " href="#">Download the app</a>
  <!-- or assign class at end -->
  <a class="btn btn-default btn-lg hidden-xs" href="#" >Text me the link</a>
  <a href="#" class="btn btn-sm btn-default"></a>
</p>
```

4.   
we'll need to toggle the navbar menu in mobile devices. Add the data attribute that calls the collapse JavaScript plugin function to the button element.
**class="navbar-toggle"*** && **data-toggle="collapse"**

the data attribute that toggles the nav once the menu icon is clicked.

**data-target=".navbar-collapse"**

```html
<div class="navbar navbar-inverse navbar-fixed-top">
      <div class="container">
        <button type="button" class="navbar-toggle" data-toggle="collapse" data-target=".navbar-collapse">
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
```

5.
> "And instead of an href attribute, it's always better to give it a data-target attribute with a hash as its value... What this data attribute does... k eeps the URLs
intact, since we're not linking to any pages with this link. We're just using it as a trigger. So now that we have our dropdown defined in our data attributes." -Guil Hernandez

Better to use data-target instead of href.
