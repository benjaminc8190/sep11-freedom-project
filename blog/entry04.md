# Entry 4
##### 3/1/24

## **Context**:

I continued to learn my tool and my partners' tools to contribute to the freedom project. Ever Since February, I have been learning some more React, but I've been shifting towards firebase from [Youtube video on connecting React withj Firebase](https://www.youtube.com/watch?v=ad6IavyAHsQ) to learn firebase features for React and to further my knowledge with React, I articulated ideas with Sam while advancing the MVP.

## **Content**:

Since my last blog, I have been trying to learn to connect my tool with my partners' tool. As a result, I came across a video on [Installing Firebase to React Project](https://www.youtube.com/watch?v=_KN_eCnZgOA) and to further my knowledge on React, I researched using [routers](https://www.w3schools.com/react/react_router.asp). 

I practiced using multiple pages so that for the Ricegrades website, I can have a student page for students to view their grades and teacher page for inputting grades, as well as an administrator page to admit students and teachers into the website. From researching the website, I started off with this:
```js
<Routes>
  <Route index element={<Home />} />
  <Route path="/blog" element={<Blogs />} />
  <Route path="/contact" element={<Contact />} />
</Routes>
```
```js
<BrowserRouter>
  <Routes>
    <Route index element={<Home />} />
    <Route path="/blog" element={<Blogs />} />
    <Route path="/contact" element={<Contact />} />
  </Routes>
</BrowserRouter>
```

However, I was curious about why the `<BrowseRouter>` is need because we already have the routes wrapped around `<Routes></Routes>`, so I deleted the `<BrowseRouter>` and it wasn't showing a change on the url. It turns out that the use for `<BrowseRouter>` is to update the url of the website for the user to know which page they are in. With this, I was able to add to my website multiple pages:

```js
<BrowserRouter>
  <Routes>
    <Route index element={<Home />} />
    <Route path="/developers" element={<Developers />} />
    <Route path="/changelog" element={<ChangeLog />} />
    <Route path="/student" element={<Student />} />
    <Route path="/teacher" element={<Teacher />} />
    <Route path="/support" element={<Support />} />
    <Route path="*" element={<NoPage />} />
  </Routes>
</BrowserRouter>
```

So far, progress of Ricegrade has been steady, we got the Home page functioning and we're in the procress of learning more css so we can make the website without the aid of Bootstrap. As we are nearing the completion of the front end of the website, we are preparing for firebase to be installed and are deciding on how we should use Firebase during the expo. 

## **EDP**:
This is the fourth step of the engineering design process. My partners and I are currently planning out who will be responsible for which parts of the project. For example, Samuel wants to practice his new css skills swaying away from frameworks like Bootstrap while me and Yu plan to installing Firebase then work on how we want the students and teachers to be admitted, and how the grades should be proccessed and displayed. Next blog, we should be finishing the MVP(most viable product) which is the fifth step of the engineering process, protoype.


## **Skills**:
Throughout this blog, I have been practicing **consideration** and **collaboration**. For our project, we have considered our competition such as PupilPath and Syncgrades because we plan to make our website look better and have a better support system. While working towards the MVP, I noticed that Sam has removed Bootstrap and moved on to making his own css. I asked him about it and he said that he feels better making it from scratch practicing what he learned about css methods such as the flexbox. Inspired by this, I adovcated for refactoring his code because I noticed that he used the same @media mulitple times not realizing it thus I shortened some of the css and learned flexbox.

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
