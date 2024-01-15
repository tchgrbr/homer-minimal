<img src="/data/icons/logo.png" width="96" align="right" />

# Homer Minimal

Homer Minimal is a clean and aesthethic theme for the [Homer Dashboard](https://github.com/bastienwirtz/homer) with support for dark and light mode and a wide range of customizations.

**Features:**
- Custom font: Inter
- Custom icons
- More spacing between cards
- Rounded Borders
- Simplified Header
- No shadows

## Preview

<p align="left">
 <details open>
  <summary>Dark mode</summary>
   <img alt="Homer Minimal" src="https://raw.githubusercontent.com/tchgrbr/homer-minimal/main/preview-dark.png">
 </details>
 <details>
  <summary>Light mode </summary>
   <img alt="Homer Minimal" src="https://raw.githubusercontent.com/tchgrbr/homer-minimal/main/preview-light.png">
 </details>
</p>

## Usage

**Important:** Make sure to create a backup of your assets folder before making any changes. You can simply copy the folder to another destination.

### File Explorer

Download and extract [this repo](https://github.com/tchgrbr/homer-minimal).

Move the content of the `assets` folder into your Homers `www` folder.

### Terminal

Clone [this repo](https://github.com/tchgrbr/homer-minimal). You can do this by running:

```sh
$ git clone https://github.com/tchgrbr/homer-minmal.git
```

Now cd into the newly created folder.

```sh
$ cd Homer-Theme
```

And now for the final step move the `assets` folder into your Homers `www` folder.
You can find this directory by running

```sh
$ sudo docker inspect -f '{{ .Mounts }}' homer
```

Move the folder by running

```sh
$ sudo mv assets /homer/www
```
_Make sure you replace `/homer/www` with the location of **your homers** www folder._

#### Go to your Homer-Dashboard IP and port and see the result!

## Customization

General customization is the same as in the vanilla version of Homer. Check out the [Github Repo](https://github.com/bastienwirtz/homer) for further instructions.

### Icons
The icons used are the ones from [Boxicons](https://boxicons.com/).
You can search the website for replacements and configure them in the `config.yaml`

The icon definition should look like this: `bx bxs-pear`

### Fonts
The standard font for Homer Minimal is [Inter](https://rsms.me/inter/). You can customize it as you wish by uploading custom webfonts to the `fonts` folder and adapting the paths in the `custom.css`.

**Example:**

```css
@font-face {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 400;
  src: url('./fonts/Inter-Regular.woff2');
  src: local(''),
       url('./fonts/Inter-Regular.woff2') format('woff2'),
}
```

### Colors
All the colors are defined in `config.yaml`, including some newly added variables, which aren't defined in the inital version of Homer. Usage is the same: You can change them by simply editing the HEX-Values. You can change them independently for dark and light mode.