# EVOLV Coaching

Online fitness coaching op maat voor afvallen, droogtrainen en spiermassa opbouwen.

## Vercel Speed Insights

This project includes Vercel Speed Insights to track web performance metrics.

### How it works

Speed Insights is integrated using the `@vercel/speed-insights` package:

1. The `injectSpeedInsights()` function is called in `speed-insights.js`
2. The script is bundled using esbuild into `dist/speed-insights.min.js`
3. The bundled script is loaded in `index.html` before the closing `</head>` tag

### Build

To build the Speed Insights bundle:

```bash
npm install
npm run build
```

### Deployment

When deploying to Vercel:

1. The build command (`npm run build`) will automatically run
2. Speed Insights will start collecting data once enabled in your Vercel dashboard
3. Go to your project settings on Vercel and enable Speed Insights

### Development

Speed Insights does **not** track data in development mode, so it won't affect local development.

## License

ISC
