# Installation

```
npm install lari-lazy-image
```

# Usage
```html
<template>
    <div>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum, repudiandae, voluptatum! Alias blanditiis consequatur dolor doloremque eligendi error esse ex fuga natus nostrum quae quaerat temporibus totam, veniam vitae voluptate.</p>
        <img src="/{your small image}.jpg" is="lazy-image"  width="{width}" height="{height}" alt="Alt tekst" small="/{your small image},jpg" normal="/{your normal image}.jpg">
    </div>
</template>
<script type="text/javascript">
    import { LazyImage } from 'lari-lazy-image'; 
    export default {
        components: {
            LazyImage
        }
    }
</script>
```

