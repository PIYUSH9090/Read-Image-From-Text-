I just write here 6 line code for read image from text.

Whenever you want you can add the image which you like you will get the text from that image.

After then you have run this program in your terminal with that location,
```
python Read-image.py
```

You can see this article via this link :- https://towardsdatascience.com/read-text-from-image-with-one-line-of-python-code-c22ede074cac

In the medium link i changed some code and getting this output well defined.

If you will use my code from my this github repo you will not get any error.

if you will use the link code directly then you will get error like this in your ubuntu system,
```
Traceback (most recent call last):
  File "Read-image.py", line 10, in <module>
    text = image_to_string(img)
NameError: name 'image_to_string' is not defined
```
solved this error from this link:- https://stackoverflow.com/questions/14640509/python-error-when-importing-image-to-string-from-tesseract/24291551
In the article you will seen there is code for windows but i did it for linux/ubuntu, So i just change the code like this.

1) First i "import image_to_string" from pytesseract.
2) Remove "pytesseract." from this line "text = pytesseract.image_to_string(img)".
