# Build Hierarchical Tree

In computer science, a tree is a widely used abstract data type (ADT)—or data structure implementing this ADT—that simulates a hierarchical tree structure, with a root value and subtrees of children with a parent node, represented as a set of linked nodes.

An example of this would be a computer's file/folder structure.

When retrieving this information from a datasource, it is being passed back unsorted in the form of the below arrays:

```
var folders = [
    { id: 5, name: "Personal", parentId: 1 },
    { id: 3, name: "Photos", parentId: 2 },
    { id: 1, name: "All Files", parentId: null },
    { id: 4, name: "Videos", parentId: 2 },
    { id: 6, name: "Documents", parentId: 5 },
    { id: 2, name: "Media", parentId: 1 },
];
var files = [
    { id: 1, name: "ToDo List.txt", folderId: 6 },
    { id: 2, name: "Course Assignment.txt", folderId: 6 },
    { id: 3, name: "Birthday.png", folderId: 3 },
    { id: 4, name: "Car.png", folderId: 3 },
    { id: 5, name: "Wedding.mp4", folderId: 4 },
    { id: 6, name: "Concert.mp4", folderId: 4 },
    { id: 7, name: "Meme.gif", folderId: 2 },
];
```
The above would display as:
* All Files
    * Media
        * Photos
            * **Birthday.png** (file)
            * **Car.png** (file)
        * Videos
            * **Concert.mp4** (file)
            * **Wedding.mp4** (file)
        * **Meme.gif** (file)
    * Personal
        * Documents
            * **ToDo List.txt** (file)
            * **Course Assignment.txt** (file)

There may be circumstances in which a given user may only have access to a portion of the file structure. In these circumstances, the unparented nodes are displayed as siblings at the highest level, and only the parented files appear.
```
var folders = [
    { id: 5, name: "Personal", parentId: 1 },
    { id: 3, name: "Photos", parentId: 2 },
    { id: 4, name: "Videos", parentId: 2 },
    { id: 6, name: "Documents", parentId: 5 },
];
var files = [
    { id: 1, name: "ToDo List.txt", folderId: 6 },
    { id: 2, name: "Course Assignment.txt", folderId: 6 },
    { id: 3, name: "Birthday.png", folderId: 3 },
    { id: 4, name: "Car.png", folderId: 3 },
    { id: 5, name: "Wedding.mp4", folderId: 4 },
    { id: 6, name: "Concert.mp4", folderId: 4 },
    { id: 7, name: "Meme.gif", folderId: 2 },
];
```
The above output would display as
* Personal
    * Documents
        * **ToDo List.txt** (file)
        * **Course Assignment.txt** (file)
* Photos
    * **Birthday.png** (file)
    * **Car.png** (file)
* Videos
    * **Concert.mp4** (file)
    * **Wedding.mp4** (file)

Challenge:
Write a function that can take either of the above two array combinations and return the hierarchical representation with the folders sorted alphabetically first, followed by the files sorted alphabetically.
