# Panorama Slider Component 🚀

A lightweight Vue 3 component for displaying a responsive, touch-enabled image slider. This component leverages SwiperJS functionality without requiring additional dependencies or installations.

## Features 🌟
- **Responsive**: Works on all screen sizes.
- **Touch-Enabled**: Swipe gestures supported out-of-the-box.
- **Pre-Bundled Assets**: No need to install or configure SwiperJS. The necessary files are already included:
  - `index.c1d53924.css`
  - `index.d2ce9dca.js`
  - `vendor.dba6b2d2.js`
- **Dynamic Images**: Easily update the image list via a JavaScript array.

## 🚀 Quick Start

### 1. Clone or Copy the Component

Clone this repository or copy the component files into your project.

### 2. Add the Required Files

Place the following pre-bundled files in your project and link them in your main HTML file:

```html
<link rel="stylesheet" href="path-to/index.c1d53924.css" />
<script src="path-to/vendor.dba6b2d2.js" defer></script>
<script src="path-to/index.d2ce9dca.js" defer></script>
```
### 3. Use the Component
```vue
<template>
  <div>
    <h1>My Image Slider</h1>
    <PanoramaSlider />
  </div>
</template>

<script setup>
import PanoramaSlider from './components/PanoramaSlider.vue';
</script>
```

## 📂 Directory Structure Example

Here’s an example of how to organize your files:

```plaintext
src/
├── assets/
│   └── media/
│       ├── 1.jpg
│       ├── 2.jpg
│       └── ...
│    └── css/
│        ├── index.c1d53924.css
│    └── js/
│        ├── index.d2ce9dca.js
│        ├── vendor.dba6b2d2.js
├── components/
│   └── PanoramaSlider.vue
├── App.vue
├── main.js
```

## 🎨 Styling

The component’s CSS is scoped for easy customization. You can modify the following classes to fit your design needs:

- **`.panorama-slider`**: Adjust container dimensions.
- **`.swiper-slide img`**: Customize image size or `object-fit` behavior.

 
 ## 🌐 Browser Compatibility

The Panorama Slider Component works on all major browsers:

- ✅ **Chrome**
- ✅ **Firefox**
- ✅ **Safari**
- ✅ **Edge**

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork this repository.
2. Make your changes.
3. Open a pull request.


## 🖼️ Demo

![5904407132722283082](https://github.com/user-attachments/assets/0301dc9e-5c52-4e3f-9cc5-8715edac29f4)



## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
