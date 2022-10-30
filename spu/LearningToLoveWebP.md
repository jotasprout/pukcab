# Learning to Love WebP

Reading time: 15 minutes | Coding time: 5 minutes

## Table of Contents

- Why You Hate WebP
- Why You'll Love WebP
- What WebP can't do
- Converting images to and from WebP
- Browser Support

### Complexity

- Worst case time complexity:
- Average case time complexity:
- Best case time complexity:
- Space complexity:

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

## What WebP Can't Do

WebP isn't yet welcome at image sharing sites like imgur **(CHECK THIS)** or Instagram **(CHECK THAT TOO)** or Flickr **(AND THAT)**. Having said that, Google created WebP so YouTube (owned by Google) plays well with WebP for banner images and thumbnails. **WHAT ABOUT GOOGLE PHOTOS?**

## Implementations

### Creating/Converting images to and from WebP

- The [official Google page for WebP](https://developers.google.com/speed/webp) includes links to tools and libraries (Windows, MacOS, Linux) for encoding, decoding, viewing, and animating the WebP format.
- As of version 23.2, Photoshop natively supports opening, creating, editing, and saving WebP but doesn't provide support for previewing when saving or for animation. One thing that makes this great news is you can batch convert oodles of images from the originals instead of using a tool or service that only converts from already compressed/degraded JPGs.
- If you're like me and don't want to upgrade to the latest version of Photoshop for whatever reason, you can use Google's WebPShop plug-in and use it with an older version of Photoshop *or the current version of Photoshop* because the plug-in fills in the gaps still remaining in Photoshop. Find instructions for installing and using the plug in at:
  - [Adobe](https://helpx.adobe.com/photoshop/kb/support-webp-image-format.html)
  - [Google](https://developers.google.com/speed/webp/docs/webpshop)

## Using WebP in Your Website

> "Setting up a website to serve WebP images is ... frustratingly ... more complicated than it should be."

I doubt the above statement is true. A simple browser check should do it.

For single code use markdown as follows:

```cpp
<picture></picture>
```

### Browser Compatibility

Not **Safari** or **Internet Explorer**?

So you must use both WebP and either JPG or PNG versions for universal compatibility but experienced devs will be used to similar situations.