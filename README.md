jquery.beyondsocial.js
======================

jquery plugin for social network feeds

[Examples & Demo](http://beyondthestatic.github.io/jquery.beyondsocial.js)
-------------------------------------------------------------------------

Usage
-----
1) link jquery.beyondsocial.js and mustache.js in your html document \
2) call the function through an empty div element with an id of your choice

Minimal Example
----------------
Displays the latest four entries of our tumblr blog.
```html
<div id="display"></div>
```
```js
$('#display').beyondsocial({ networks: [{name:'tumblr', id:'beyond-t-s'}] });
```

Settings
--------
Default Settings:
```js
{
  networks: [{name: 'tumblr', id: 'beyond-t-s'}, {name: 'facebook', id: '323476337711540'}],
  maxResults: 4.
  template: "mustache/rss.mustache",
  bulkload: true
}
```
Possible Values:
```js
{
  networks: [{name: 'tumblr' | 'facebook' | 'pinterest' | 'instagram' 
                id: valid id according to the social network you choose
            }, ...],
  maxResults: greater than 0, whole numbers
  template: valid path to your template file
  bulkload: true | false
}
```
