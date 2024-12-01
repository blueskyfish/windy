
![Windy](logo-144.png)

# Windy

> Standard CSS styles for hectic and windy development work.
> 
> 🚧 Project is under construction...

## Motivation

When developing a web application, it is important to design the code as efficiently and clearly as possible.
Unfortunately, it often happens that when creating CSS classes, you repeatedly use the same properties and values.
This can quickly make the code confusing and difficult to maintain.

To address this problem, it makes sense to outsource the common properties into reusable classes or mixins.
This allows the code to be much more compact and readable. It also facilitates later changes, as you only need
to make adjustments in one place.

By using technologies like Sass or Less, developers can also further improve the modularity and structure of
their CSS code. This creates a clean, maintainable codebase that is easy to expand, even for complex web
applications.

### Example

```css
.app-title {
    align-items: center;
    display: flex;
    flex-direction: row;
    flex-wrap: nowrap;
    
    .title {
        flex: 1 1 auto;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
    }
    .icon {
        flex: 0 0 auto;
        margin-right: 0.5rem;
    }
}
```

*The CSS declarations are repeated in this and a similar way*

Wouldn't it be nice if this could be done using simple CSS classes?

```html
<h1 class="wy-align-center wy-flex wy-flex-nowrap wy-flex-row">
    <span class="icon wy-flex-shrink wy-me-2">...</span>
    <span class="title wy-flex-grow wy-truncate">...</span>
</h1>
```


## Install

TBD

## Information

> To make the CSS classes easy to use, here is some information

| Name    | Description                                          |
|---------|------------------------------------------------------|
| **wy**  | The CSS classes use the prefix **wy**.               |
| **gap** | The distances are counted in **0.25rem** increments. |



## Include in your Project

TBD


## License

```text
MIT License

Copyright (c) 2024 BlueSkyFish

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```