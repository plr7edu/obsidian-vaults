## What Is An Embedded Query?

- In Obsidian, an embedded query is functionality that lets you insert a search query into a note. 
- You’ll then see the results of the query display from directly within the note.

- Think of it like a saved search that you don’t have to type into the search bar every time you need it.

- This is useful if you’d like to retrieve lists of specific notes on a regular basis.

- This is core Obsidian functionality which means you don’t have to install any community plugins to make it work.

## How Can I Set Up An Embedded Query?

To set up an [embedded query](https://help.obsidian.md/Plugins/Search#Embed+search+results+in+a+note) in a note you’ll need to:

1.  Create a [code block](https://help.obsidian.md/How+to/Format+your+notes#Code+blocks) which is three opening and three closing backticks.
2.  After the first three backticks, you add the term query to denote this is a search query.
3.  Enter a search term into the code block. You can build a search term using the search bar and copy the search in here.
4.  If all is working correctly you should see a list of notes that match the search term you entered! (See the code snippet below as an example).

````
```query
file:("Daily Note")
```
````

## Pros And Cons Of Embedded Queries

I realize this approach may not be for everyone so I wanted to highlight some of the pros and cons of using embedded queries over using something like Dataview.[^1]

[^1]: Later we talk about it.

### Pros:

-   Much simpler to use than a plugin like Dataview.
-   You can build a search query using the search bar and simply copy it into the query code block.

### Cons:

-   As it’s simpler than Dataview[^1] you’re missing a lot of the functionality of something as powerful as Dataview. For instance you can only retrieve lists not tables.

[[Plugin Notes Search Query|Query Sample]]

[[4 - Obsidian Query Control Plugin]]

