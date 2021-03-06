# Invalid images config

#### Why This Error Occurred

In your `next.config.js` file you provided an invalid config for the `images` field.

#### Possible Ways to Fix It

Make sure your `images` field follows the allowed config shape and values:

```js
module.exports = {
  images: {
    // limit of 25 deviceSizes values
    deviceSizes: [320, 420, 768, 1024, 1200],
    // limit of 25 imageSizes values
    imageSizes: [],
    // limit of 50 domains values
    domains: [],
    path: '/_next/image',
    // loader can be 'default', 'imgix', 'cloudinary', or 'akamai'
    loader: 'default',
  },
}
```

### Useful Links

- [Image Optimization Documentation](https://nextjs.org/docs/basic-features/image-optimization)
