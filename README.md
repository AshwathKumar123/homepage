# Homepage
My browser homepage repository, with the nord color scheme. Hosted on GitHub pages for everyone to use. [GitHub Pages Link](https://vyzicgithub.github.io/homepage/)

![Screenshot of homepage](https://github.com/VyzicGithub/homepage/blob/main/homepage-screenshot.png)

Forked from [JaredK3nt/homepage](https://github.com/JaredK3nt/homepage), with color scheme and font changes.

### Customization

#### Customize Bookmarks

Bookmarks are now held in the `bookmarks.js` file for easy updating. `bookmarks` is an array of objects with a `title` and `links` property. The `title` defines what the header of the "bookmark section" box will be. `link` is an array of link objects each with a name and a url to link to.

> The way the site is currently styled bookmarks should always have a length of `4` if you want to have more sections you need to change the `width` property of the css class `bookmark-set`

### Customize Search Engine

You can change the search engine used by the search overlay by updating the url value stored in the `searchUrl` var in `index.html` to the correct string for your engine.

Examples:

- DuckDuckGo: `https://duckduckgo.com/?q=`
- Bing: `https://www.bing.com/search?q=`

### Customize Styling

Styles are handled through CSS variables. To update the colors you just need to change the variable definitions defined in `:root`.

| Variable           | default                    | description                                                                                                                |
| ------------------ | -------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| `--bg`             | `#2e3440`                  | Defines the body background color |                                                                                          
| `--fg`             | `#ffffff`                  | Defines the primary foreground (text) color for clock, weather, and titles |                                          
| `--secondaryFg`    | `#717682`                  | Defines the foreground (text) color for links |                                                                              
| `--containerBg`    | `#1d2128`                  | Defines the background color of the boxes |                                                                                
| `--searchBg`       | `#2e344`                   | Defines the background color of the search overlay |                                                                         
| `--scrollbarColor` | `#3f3f3f`                  | Defines the color of the custom scrollbars |                                                                                  
| `--fontFamily`     | `"Product Sans", Normal` | Defines the font used. To change to a custom font you will also have to import that font from whatever source is available |
