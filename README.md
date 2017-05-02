# es-plugin

## Description

The web has had a long history of different ways to create components for our websites and web applications. Gone are the days where websites were created of “pages”. Websites and web application are more demanding than ever. Using components to create reusable code has been goal that we haven’t quite achieved. We have seen components like jQuery’s plug-in api, Angular Directives, React components and more. They all try to accomplish the same goal but do it in different ways. We need a common browser API standard.

One of the main issues in our components today are style conflicts. This is when our CSS or the imported component breaks CSS somewhere else. Another is lack of native templating of HTML. Storing HTML templates on a page have only been possible by using script tags or other hacks. The current component structures lack of semantic meaning. We end up with a big pile of div’s that have little meaning. Angular has tried to help this with its custom element directives.

The new HTML5 [Web Component Specification](https://www.webcomponents.org/introduction) is a collection of specifications that when combined create a powerful web standard for creating reusable components.

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install es-plugin --save
```


## Usage

1. Import polyfill:

    ```html
    <script src="bower_components/webcomponentsjs/webcomponents.min.js"></script>
    ```

2. Import custom element:

    ```html
    <link rel="import" href="bower_components/es-plugin/es-plugin.html">
    ```

3. Start using it!

    ```html
    <es-plugin></es-plugin>
    ```

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

1. Install [bower](http://bower.io/) & [polyserve](https://npmjs.com/polyserve):

    ```sh
    $ npm install -g bower polyserve
    ```

2. Install local dependencies:

    ```sh
    $ bower install
    ```

3. Start development server and open `http://localhost:8080/components/my-repo/`.

    ```sh
    $ polyserve
    ```
