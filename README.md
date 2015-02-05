# Filter Collection Library for Backbone
The Filter Collection allows use to filter a collection and have it update the internal collection and triggers a `filter` event.

## Usage 
Include the file after Backbone is loaded and create a collection with it using:

```javascript
var collection = new Backbone.FilterCollection.extend();
```

To filter the collection:

```javascript
collection.addFilter("nameOfFilter", function (model) {
    // return true if this model should remain in the collection
    // return false if this model should be filtered out of the collection
});
```

