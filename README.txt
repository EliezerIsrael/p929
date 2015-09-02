# p929

Tools for the [Project 929](http://929.org.il) chapter-a-day reading of Tanach.
Get the Perek for today, or any other day, and then data and URLs for that Perek. 

(Note - this code is not an official 929 project.)

## Attributes of a `Perek` object
* `date`: `datetime.date` object of this Perek's date.
* `book_name`: String name of the book that this Perek is found in
* `book_chapter`: Integer number of the chapter in the book
* `number`: Perek number, counting from beginning of Tanach
* `hashtag`: Project 929 hashtags for this Perek
* `url_929`: URL of this Perek on 929's website
* `url_sefaria`: URL of this Perek on Sefaria.org's website

## Example usage
Getting today's perek (on September 2nd, 2015)
```
>>> import p929
>>> p = p929.Perek()
>>> vars(p)
{ 'as_a_phrase': 'Perek for Wednesday 02 September 2015 is #184: Deuteronomy 31',
 'book_chapter': 31,
 'book_name': u'Deuteronomy',
 'date': datetime.date(2015, 9, 2),
 'hashtag': '#p929 #ch184',
 'number': 184,
 'url_929': 'http://www.929.org.il/page/184',
 'url_sefaria': 'http://www.sefaria.org/Deuteronomy.31'}
```
