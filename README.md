# webpack-plugins-collection
收集webpack plugins
#### workbox-webpack-plugin

这是webpack生成PWA的插件

```javascript
new WorkboxWebpackPlugin.GenerateSW({
    clientsClaim: true,
    exclude: [/\.map$/, /asset-manifest\.json$/],
    importWorkboxFrom: 'cdn',
    navigateFallback: publicUrl + '/index.html',
    navigateFallbackBlacklist: [
        new RegExp('^/_'),
        new RegExp('/[^/]+\\.[^/]+$'),
    ],
}),
```
