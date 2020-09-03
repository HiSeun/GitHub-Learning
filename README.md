# Github Markdown Learning
## 1. Header Usage Method

### 1.1.Using ======
================

### 1.2.Using ------
----------------

## 2. BlockQuote
We can use '>' block letter.

> This is a first blockquote.
> > This is a second blockquote.
> > > This is a third block quote.

## 3. List

### 3.1. Using sequence number
We use 1.~~ 2. ~~~ 3.~~~
Whether we changes as 1.~~ 3.~~ 2.~~~ It shows 1. 2. 3. sequence.

1. First list
3. Second list
3. Third list

### 3.2. Without sequence number
Using '*', '-', '+'
* for '*'
    - for '-'
        + for '+'
            * also for '*'
        
## 4. Codeblock
We can use two methods to make codeblock.
### 4.1. ```<pre><code>{code}</code>/pre>``` Method 

<pre>
<code>
public class BootSpringBootApplication {
    public static void main(String[] args) {
        System.out.println("Hello, Everyone");
    }
}
</code>
</pre>

### 4.2. "```" Method

```
public class BootSpringBootApplication {
    public static void main(String[] args) {
        System.out.println("Hello, Everyone");
    }
}
```

## 5. Horizontal line 

* "* * *" 
* * *
* "***"
***
* "- - -"
- - -
* "----------"
----------------
* ```<hr/>```
<hr/>

## 6. Link
### 6.1. Reference Link

```
[Link Keyword][id]
    [Link Keyworld] is equal to [Naver]   
    [id] contains two arguments which are -- URL "Optional Title"
        This optional title shows the optional title when you brings your cursor on to the link.
```
* Not using optional title example
```
Link1 : [Naver][https://www.naver.com]
```
Link1 : [Naver][https://www.naver.com]

* Using optional title example
```
Link2 : [Youtube][YoutubeId]
[YoutubeId]: https://www.youtube.com "Go youtube"
```
Link2 : [Youtube][YoutubeId]
[YoutubeId]: https://www.youtube.com "Go youtube"

### 6.2. External Link

* Using optional title example2
```
[Title](link)
[Google](https://google.com, "google link")
```
[Google](https://google.com, "google link")

### 6.3. Use proper type

* For external link
``` 
External link : <http://example.com>
```
External link : <http://example.com>

* Email link
```
Email link : (address@example.com)
```
Email link : (address@example.com)

## 7. Emphasis
If you want to use this in the middle of the sentence, you should use 'space bar' to make blank between others.

```
*single asterisks*
```
- *single asterisks*
```
_single underscores_
```
- _single underscores_
```
**double asterisks**
```
- **double asterisks**
```
__single underscores__
```
- __single underscores__
```
~~cancelline~~
```
- ~~cancelline~~

## 8. Inserting Image

* If you use "Optional title", you can see the title when the cursor is on the image. 
```
![Alt text](/path/to/image.jpg)
![Alt text](/path/to/image.jpg "Optional title")
```

* Since there is no other properties for size, you should use ```<img width="" height ""></img>``` .

```
<img src = "/path/to/img.jpg" width = "~px" height = "~px" title = "~~~" alt = "~"></img><br/>
<img src = "/path/to/img.jpg" width = "~%" height = "~%" title = "~~~" alt = "~"></img>
```

## 9. Line change
If you make 3 or more blanks at the end of the sentence, the line changes.
```
You should make at least three blanks to change the line.  not  Like this.
You should make at least three blanks to change the line.       Like this.
```
You should make at least three blanks to change the line.  not  Like this.
You should make at least three blanks to change the line.       Like this. 
