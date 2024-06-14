1. Preset App.test.js do not work for your project, need to change based on your need.
2. screen: allows you to access elements rendered in the document without needing to directly reference the container. This simplifies and clarifies the test code.
3. Accessible by Everyone, Semantic Queries, Test ID














































| Method          | Returns                     | Throws Error on Failure | Async | Use Case                                                                                                                                                                                                                  |
| --------------- | --------------------------- | ----------------------- | ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `getBy...`      | Single element              | Yes                     | No    | To get an element that must be present in the DOM. Throws an error if no matching element is found or if multiple elements are found.                                                                                     |
| `queryBy...`    | Single element or `null`    | No                      | No    | To check if an element is present or absent in the DOM without throwing an error. Returns `null` if no matching element is found. Throws an error if multiple elements are found.                                         |
| `findBy...`     | Single element (Promise)    | Yes                     | Yes   | To get an element that may not be present initially but will appear eventually. Returns a Promise that resolves when the element is found. Throws an error if no matching element is found within the timeout.            |
| `getAllBy...`   | Array of elements           | Yes                     | No    | To get multiple elements that must be present in the DOM. Throws an error if no matching elements are found.                                                                                                              |
| `queryAllBy...` | Array of elements or `[]`   | No                      | No    | To check if multiple elements are present or absent in the DOM without throwing an error. Returns an empty array if no matching elements are found.                                                                       |
| `findAllBy...`  | Array of elements (Promise) | Yes                     | Yes   | To get multiple elements that may not be present initially but will appear eventually. Returns a Promise that resolves when the elements are found. Throws an error if no matching elements are found within the timeout. |
