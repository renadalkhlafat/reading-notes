# NextJs
- **Assets :**  Next.js can serve static assets, like images, under the top-level public 
    + Using the Image Component: Instead of optimizing images at build time, Next.js optimizes images on-demand, as users request them. Unlike static site generators and static-only solutions

- **Metadata :** Like title tag, refers to the text that is displayed on search engine result pages and browser tabs to indicate the topic of a webpage

- **Css :** This page is using a library called styled-jsx. It’s a “CSS-in-JS” library — it lets you write CSS within a React component, and the CSS styles will be scoped

## React Context
a method to pass props from parent to child component(s), by storing the props in a store(similar in Redux) and using these props from the store by child component(s) without actually passing them manually at each level of the component tree

it is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context