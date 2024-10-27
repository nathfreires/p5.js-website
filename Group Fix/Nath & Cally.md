# Progress Report on p5.js Website Project

## Bug Chosen
- **Issue**: [Bug #516](https://github.com/processing/p5.js-website/issues/516)

## Technical Overview
This is a bug where the text gets cropped and no longer legible on smaller screen sizes.
## Expected Behavior
Text should remain legible and not crop, no matter what device or browser you’re using.
### Getting Started with Development

#### Setup
1. **Prerequisites**: Ensure you have Node.js and npm installed on your machine.
2. **Clone the Repository**: 
   ```bash
   git clone https://github.com/processing/p5.js-website/
3. npm install
4.npm run dev

Then it will show your local host, example http://localhost:4321/.

Inspected the website and found a class with the following styles:
class="mt-0 col-span-2 lg:col-span-3 lg:text-3xl md:text-xl text-md"

Attempted to locate the style in VSCode but couldn't find it initially.

Used the browser's network tool and I found this:
CSS File: https://p5js.org/_astro/about.BCl6XkZR.css

Found the following in my local environment:
data-astro-source-file="C:/Users/Nath/p5.js-website/src/components/PageHeader/HomePage.astro"

Located the HomePage.astro file in VSCode and we started tweaking styles and components.

