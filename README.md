# Handmade Isolated Bootstrap 3.3.5
All the thing I did here is a simple use of Less to bind all of Bootstrap 3.3.5 dist to a HTML class

# Solution
<p align="center">
    <img src="https://lesscss.org/public/img/less_logo.png" width="100px;"/>
</p>

- First thing, you need to install Less and there are many ways to do so and I use `npm`
```
npm install less --global
```
- You may not use it immediately cause the path is not set to it so, you need look for the `bin` in `node_modules` from your `User` folder. Look for it with this path: 
```
C:\Users\Name_of_your_user\AppData\Roaming\npm\node_modules\less\bin
```
Then add it to your Path Management

- Create `prefix.css` in the same place with `boostrap.min.css` and import it in

```less
.bootstrap-iso {
    @import (less) 'bootstrap.min.css';
}
```
- Open terminal in that place and run line
```bash
lessc prefix.less bootstrap-335-iso.css
```

Then you will notice a new file named `bootstrap-335-iso.css` created.

## Usage

1. Replace the normal Bootstrap link with one of these in the head of a HTML page.

```html
<link rel="stylesheet" href="path_to_your_bootstrap_iso">
```

2. Include `class="bootstrap-iso"` where you want to use Bootstrap styles.

3. You are ready to go, adios

```html
<!-- there Bootstrap doesn't work -->
<div class="bootstrap">
    <!-- there Bootstrap works-->
</div>
<!-- there Bootstrap doesn't work-->
```
