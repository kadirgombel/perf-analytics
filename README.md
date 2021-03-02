# Performance Analytics

> Performance analytics tool for TTFB, FCP, Dom Load, and Window Load events

## Install

```
$ npm install git+https://github.com/kadirgombel/perf-analytics.git
```

## Usage

```js
import perfAnalytics from 'perf-analytics';

const saveUrl = 'http://localhost:3030/analytics';
const perfAnalyzer = perfAnalytics({ url: saveUrl });

perfAnalyzer.run();
```

## API

### perfAnalytics(options?)

#### options

Type: `object`
```js
{
  TTFB = true, // Calculate Time To First Byte time
  FCP = true, // Calculate First Contentful Paint time
  domLoad = true,  // Calculate DOM Load time
  windowLoad = true, // Calculate Window Load time
  resourceLoad = true, // Calculate Resources Load time
  url = 'http://localhost:3030/analytics' // Save endpoint url - POST
}
```
## Commands

- `npm run clean` - Remove `lib/` directory
- `npm run lint` - Run ESlint with airbnb-config
- `npm run build` - Babel will transpile ES6 => ES5 and minify the code.
- `npm run prepublish` - Hook for npm. Do all the checks before publishing your module.


## License

MIT © Kadir Gombel
