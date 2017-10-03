# html5-image-srcset

### image srcset for responsive images

This is useful for when you want to change images depending on which device or width of the browser users are on.
It is simply updating images from a list specified in the srcset attribute together
with a w (stands for width and are same as pixels).


### Example:

```
<img src="large.jpg" srcset="small.jpg 450w, medium.jpg 767w, large.jpg 1024w" alt="my cat" />
```

### or with picture:

```
<picture>
    <source srcset="small.jpg 450w, medium.jpg 767w, large.jpg 1024w" />
    <img src="large.jpg" alt="my cat" />
</picture>
```

### You can also add media attribute or sizes:

```
<img src="large.jpg" srcset="small.jpg 450w, medium.jpg 767w, large.jpg 1024w" alt="my cat" sizes="(min-width: 450px) 450px"/>
```

```
<picture>
    <source srcset="small.jpg" media="(min-width: 450px)"/>
    <img src="large.jpg" alt="my cat" />
</picture>
```

FYI If you are using srcset directly on the image you need to reload the image in diffrent breakpoints.
