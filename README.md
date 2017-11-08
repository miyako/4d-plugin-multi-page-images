# 4d-plugin-multi-page-images
Basic tool for GIF, TIFF, PDF

### Platform

| carbon | cocoa | win32 | win64 |
|:------:|:-----:|:---------:|:---------:|
|||||

### Version

<img src="https://cloud.githubusercontent.com/assets/1725068/18940649/21945000-8645-11e6-86ed-4a0f800e5a73.png" width="32" height="32" /> <img src="https://cloud.githubusercontent.com/assets/1725068/18940648/2192ddba-8645-11e6-864d-6d5692d55717.png" width="32" height="32" />

[``libgd``](https://github.com/libgd/libgd) and [``libtiff``](http://www.simplesystems.org/libtiff/) for ``GIF`` and ``TIFF``. [``libgs``](https://ghostscript.com/) for ``PDF``.

---

## Syntax

```
count:=TIFF Count pages (image)
```

param|type|description
------------|------|----
image|PICTURE|
count|LONGINT|number of images

```
TIFF GET PAGES (image;images{;start{;end}})
```

param|type|description
------------|------|----
image|PICTURE|
images|ARRAY PICTURE|images
start|LONGINT|``1`` is first page. negative number means offset from last page
end|LONGINT|negative number means offset from last page

```
image:=TIFF Create from array (images)
```

param|type|description
------------|------|----
image|PICTURE|
images|ARRAY PICTURE|images
