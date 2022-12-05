# fabulous-text-editor

## Description

Here we have a wonderful, wonderful text editing app [Here is a link to the application](https://warm-fortress-57567.herokuapp.com/)
A user may save and edit their text with it.


## How to use

It is very intuitive on how to use. Just pop it up and enjoy!

## Screenshot of app result

![screenshot](https://cdn.discordapp.com/attachments/408481106040717322/1049131883679719594/image.png)

## the Code!

```
export const getDb = async () => {
  const jateDb = await openDB('jate', 1);
  const trans = jateDb.transaction('jate', 'readonly');
  const store = trans.objectStore('jate');
  const request = store.get(1); //had to change from getAll to get(1)
  const result = await request;
  // console.log('retrieving the things', result.value)
  return result?.value
};
```

## Author Links
[Linkedin](https://www.linkedin.com/in/dominic-conradson-76638b172/)---
[GitHub](https://github.com/theDomConrad/)---
[Portfolio](https://thedomconrad.github.io/Dominic-Conradson-Portfolio/)---

