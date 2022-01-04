# keystone6-documentreader-vue

This is a Vue version of the DocumentReader component for Keystone 6. The version supplied by Keystone is React only so I wrote this version that uses Vue (2, but should work in 3).

**IMPORTANT: I am experiencing issues compiling this package due to Vue/JSX issues. If anyone can assist with this please see [this issue](https://github.com/craigharman/keystone6-documentreader-vue/issues/2). In the meantime you can download the entire source code to your project and import directly: `import KeystoneDocument from 'keystone6-documentreader-vue/src'`**

## Usage

Install the npm package:

```bash
npm install keystone6-documentreader-vue
```

Then in your Vue component/page:

```js
import KeystoneDocument from "keystone6-documentreader-vue";

export default {
	components: {
		KeystoneDocument,
	},
};
```

Then use the component in your Vue template:

```html
<KeystoneDocument :document="$page.content.document" />
```

Where `document` is a Keystone 6 document object from your GraphQL query.
