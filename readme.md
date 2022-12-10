# thirdweb-sdk tree shaking issue (vite)

There's something wrong with how the exports are done in thirdweb-sdk which causes the treeshaking to not work properly.

## Install dependencies

```bash
npm install
```

## Create a Build

```bash
npm run build
```

## Preview the App

```bash
npm run preview
```

Open the Network panel in the browser and you'll see that a lot of unnecessary code is loaded

<br/>

## Try different imports

Go to main.js and try importing different stuff to see how the bundle size changes.

### Example

```javascript
import { ChainId } from '@thirdweb-dev/sdk/evm';

console.log(ChainId);
```
