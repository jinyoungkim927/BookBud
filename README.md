# BookBud
Ever stood before a bookshelf, overwhelmed by all the titles in search of the perfect fireside read? Our app can scan the books, getting reviews, ratings, and potentially cheaper prices elsewhere! iOS app written in Swift to explore Google Books API. Integrates OCR for search. 

Currently uses:
  - Alamofire
  - AlamofireObjectMapper
  - SwiftyJSON

Supports searching volumes by name and returning up to 40 found elements. 
Provides detailed info about every found element, including title, author and description. 

Uses `Volume list` request (https://developers.google.com/books/docs/v1/reference/volumes).

## Further possible improvements
- Add data loader indicator.
- Implement pagination to show all founded results (use provided `startIndex` and response's `totalItems` value).
- Implement of adaptive UI for DetailViewController (currently does not scroll, so in some cases not all content can fit the screen).
- Inherit model from `ImmutableMappable` instead of `Mappable`. 
- Add founded volumes to storage to enable offline access to them.
- Implement search filter: by language, print type (book, magazine, all), etc. 
- Implement authorization in order to have access to bookshelf.
