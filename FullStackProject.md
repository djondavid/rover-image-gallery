# Full Stack candidate project
In order to get a sense of your overall style and approach to developing web applications, we would like to see what you can do when given freedom of design but also a somewhat limited window of time.

### Overall goals:

* Using the NASA API for the Mars Rovers, please develop an image browser that loads Mars Rover photos
	- The API is fairly straightforward and all necessary documentation to start getting results is present in this page section: [NASA Open APIs](https://api.nasa.gov/api.html#MarsPhotos)
	- Your API key is: `YQv888J9gVeBN6TPQJqZ78ox127KhPQriWjNbYKa`
	- Example query to verify this API key is good: https://api.nasa.gov/mars-photos/api/v1/rovers/curiosity/photos?sol=1000&api_key=YQv888J9gVeBN6TPQJqZ78ox127KhPQriWjNbYKa
	- Example boilerplate Angular project that you could choose to use to get started: [GitHub - eventfarm/angular-CLI-starter-with-observable-service-bootstrap: Angular CLI project jumping-off-point with included RXJS Observable async API use structure, plus service, router, UI boilerplate](https://github.com/eventfarm/angular-CLI-starter-with-observable-service-bootstrap) . Alternatively you could use your own along with a different framework, we have no preference there.


### Implementation Details

**The developed Mars Rover image browser should:**
1. Offer navigation to switch between rovers either in a left-side navigation panel or a top navigation panel. Default choice can be a rover of your choosing.
2. Offer a UI (implantation details are up to you) that further allows filtering of the specific rover images by day. Such as displaying only images from today, yesterday, and two days ago from the previously-selected rover. Default filter should be for today’s images.
3. As the user clicks nav links to switch between rovers and optionally chooses non-default date filters, the main web app page body should update with a feed of photos based on the selections.
4. Below each photo, please include the timestamp of the photo as delivered by the API, as well as other metadata if available
5. Dates should be converted into a consistent human-readable format for display on the UI
6. Support for older browsers is not expected. As long as it works in the latest Chrome/Firefox (and Safari if possible) that is fine.

### Preferred architecture, frameworks, etc

1. Please develop this using a modern API-based single page web app  architecture with modular components
	* Using a static DOM with jQuery (or similar) DOM manipulations to display interactive elements is discouraged
2. This codebase generated by this project will be small, but it should be developed using patterns and data models designed to scale. Imagine this being the seed of a much larger project being actively developed by others in the future
	* Please incorporate some sort of shared data model that the individual components/modules can pull from. The Angular service feature, Redux, or a singleton class can be incorporated for storing and sharing around the API credential for instance.
3. **React, Angular, Vue, or similar are all great to use.**
	* If you would prefer to not use third-party frameworks, a framework-like architecture such as WebComponents is encouraged.
	* For reference, Event Farm is built using Angular (version 4 currently), Angular routes, and uses “vanilla” TypeScript classes for strict structuring of data objects displayed in the Angular front-end.
4. Regarding UI appearance and style/CSS: Developing attractive stylesheets takes time, so a barebones and “ugly” minimal UI is fine.
	* Using tools like Bootstrap , Foundation, or similar is encouraged to allow you create a functional UI without spending time on basic style boilerplate.

### Timeframe and Delivery

**Please do not actively develop for more than eight hours on this.** While seeing what can be developed during a limited timeframe is useful, we do not want to take up too much of your time most importantly.

When you are finished, please upload the project to your own GitHub (and then please invite @toddcornett to it), or more simply attach the project to an email to todd.cornett@eventfarm.com or tcornett@membersuite.com with installation & run instructions
