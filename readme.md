<img src="/assets/icons/logo.png" width="96" align="right" />

# Homer Minimal

Homer Minimal is a clean and aesthethic theme for the [Homer Dashboard](https://github.com/bastienwirtz/homer) with support for dark and light mode and a wide range of customizations.

**Features:**
- Custom font: Inter
- Custom icons
- More spacing between cards
- Rounded Borders
- Tags are initially hidden
- Updated Tag position
- Simplified Header
- No shadows

## Preview

<img alt="Homer Minimal Demo" src="https://raw.githubusercontent.com/tchgrbr/homer-minimal/main/homer-minimal-demo.gif">

<p align="left">
 <details>
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

### Tags
Tags are now not visible by default, only on hover. The tags can be hidden in the `custom.css` file if desired by commenting in the property. Color customization works like in the default homer version, by utilizing the `tag-style` property from Bulma CSS in your `config.yaml`.

Homer uses bulma CSS, which provides a modifiers syntax. You'll notice in the config there is a tagstyle option. It can be set to any of the bulma modifiers. You'll probably want to use one of these 4 main colors:

- `is-info` (blue)
- `is-success` (green)
- `is-warning` (yellow)
- `is-danger` (red)

