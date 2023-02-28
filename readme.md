## Getting Started with tailwind CSS

Installation 

```
npx tailwindcss init
```

- This creates a *config* file where you can tell tailwind where to look for the imported tailwind library


## Create a css file (input.css)
- Add these imports at the top of the file

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

- This is used to compile the css from this input.css file and it creates it for us inside the build directory or wherever your build directory path points to.

## Enter to following commmand 

```
npx tailwindcss -i ./src/input.css -o ./build/css/style.css

```

- This command specify our input file and our output or compiled file which contains all the tailwind styles.

## Add a Link tag to index.html pointing to css file path

```
<link rel="stylesheet" href="css/style.css">
```

## Add any basic element & for the class use tailwind properties

```
<div class="bg-emerald-500 w-52 h-52 rounded-full shadow-xl grid place-content-center">
```

- bg-emerald-500 (changes color to emerlad at 500 opacity)
- w-52/ h-52 (are both width and height respectively)
- rounded-full (will add a completed rounded cornerand create a circle)
- shadow-xl (will add a bigger shadow area)
- grid (represents `display:grid`)
- place-content-center (represents the same `place-content:center` css property)


## Demo
<img src="image/demo-01.png" alt="demo" width="50%">

### List of tailwindcss properties can be found at <a href="https://tailwindcss.com/">official documentation</a>