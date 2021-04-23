## What is an API?

A set of clearly defined **methods** of communication between various components

An API may be for a web-based system, operating system, database system, computer hardware, or software library.

- e.g. Web APIs
- Companhies will provide access to their data
  - e.g. Twitter API, Facebook API, GooglePlaces API

## Data Formats

When API request is made, APIs will respond with data in two different formats - XML and JSON

**XML**

XML may look similar to HTML, but does not describe presentation like HTML, and many of the tags are custom

```jsx
<person>
  <name>Elie</name>
  <favoriteColor>purple</favoriteColor>
  <city>San Francisco</city>
</person>
```

**JSON (JavaScript Object Notation)**

JSON also look like JS objects, but all the keys must be "double-quoted".

```json
{
  "person": {
    "name": "Elie",
    "favoriteColor": "purple",
    "city": "San Francisco",
    "favoriteNumber": -97,
    "interests": ["CEOing", "eating Mediterranean food"],
    "futureDreams": null
  }
}
```
