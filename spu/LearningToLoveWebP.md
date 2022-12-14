# Learning to Love WebP

Reading time: 15 minutes | Coding time: 5 minutes

## Table of Contents

- Why You Hate WebP
- Why You'll Love WebP
- What WebP can't do
- Converting images to and from WebP
- Using WebP in Your Website and Browser Compatibility

## Why You Hate WebP Right Now

There are few things as infuriating as right-clicking something on a web page only to discover right-clicking is disabled. You may feel, however, that the following situation comes pretty close.

> You *think* you've successfully right-clicked to download an image only to find it has the **.WebP** format, spend far more time than you'd like googling "WebP" so you can convert it, only to finally hurl your latte across the room in disgust and adding WebP to the list of things you hate.

Now that we have a common enemy -- so we're soulmates and you trust me -- let's take a look at this file format (which isn't going anywhere) and learn why you might just start using it yourself.

## Why You Will Love WebP from Now On

Think of all the reasons you choose **PNG** when you can -- transparency and crisp beauty.

Think of all the reasons you choose **JPG** when you must -- small file size that serves up fast.

### Applications

Now imagine a world with a file format that has everything you love about PNG as well as the benefits of using JPG and does all of them *even better*. Welcome to **WebP**. Using WebP means your images (and thus, your page) load faster and look prettier. WebP comes in both lossless and lossy flavors.

Oh, did I forget to mention *animation*? WebP also supports animation with smaller file size and higher quality than a **GIF**.

### What WebP Can't Do

WebP isn't yet welcome at image sharing sites like imgur or Flickr. While Facebook let me upload a WebP image, Instagram would not.

Having said that, Google created WebP so Google Photos, YouTube, and Gmail all play well with WebP.

## Implementations

### Converting images to and from WebP

- The [official Google page for WebP](https://developers.google.com/speed/webp) includes links to tools and libraries (Windows, MacOS, Linux) for encoding, decoding, viewing, and animating the WebP format.
- As of version 23.2, Photoshop natively supports opening, creating, editing, and saving WebP but doesn't provide support for previewing when saving or for animation. One thing that made this great news is you can batch convert oodles of images from the originals instead of using a tool or service that only converts from already compressed/degraded JPGs.
- If you're like me and don't want to upgrade to the latest version of Photoshop for whatever reason, you can use Google's WebPShop plug-in and use it with an older version of Photoshop *or the current version of Photoshop* because the plug-in fills in the gaps still remaining in Photoshop. Find instructions for installing and using the plug in at:
  - [Adobe](https://helpx.adobe.com/photoshop/kb/support-webp-image-format.html)
  - [Google](https://developers.google.com/speed/webp/docs/webpshop)
- A growing number of other apps such as Picasa, ImageMagick, Blender, and GIMP all welcome WebP.

### Using WebP in Your Website and Browser Compatibility

You can use the ```<img>``` tag like you would for JPG or PNG but for browser compatibility reasons alone, you should take advantage of the ```<picture>``` tag and ```srcset``` attribute instead. Experienced devs will already be used to using the following method for responsive images and websites.

The ```<picture>``` tag allows you to list alternate sources for an image. 

```html
<picture>
    <source type="image/webp" srcset="funnycatpicture.webp">
    <source type="image/jpeg" srcset="funnycatpicture.jpg">
    <img src="funnycatpicture.jpg" alt="My cat being derpy">
</picture>
```

If the browser can display the first source, it will. If not, it moves on to the next in the list. The last in the list should be an image in an ```<img>``` tag with a default, universally compatible image.
