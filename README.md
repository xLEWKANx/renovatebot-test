# Renovatebot is awesome!

## Flow
1. Added [Renovate Bot]( https://github.com/apps/renovate) to repository
2. It created a default configuration file by making a [PR](https://github.com/xLEWKANx/renovatebot-test/pull/1)
3. I [configured](https://docs.renovatebot.com/node/) renovate bot manually to update node.js by specifying `engine` in package.json (by default it updates only minor versions)
```
"engines": {
  "node": ">15.1"
}
```
4. I disabled the managing of npm packages by placing `"enabledManagers": ["circleci"]` to [renovate.json](https://github.com/xLEWKANx/renovatebot-test/blob/main/renovate.json) and the bot closed [PR with npm packages update](https://github.com/xLEWKANx/renovatebot-test/pull/2)
5. So if we want to update node.js version we need to [merge the PR](https://github.com/xLEWKANx/renovatebot-test/pull/5). Tests run automatically.

## Cool stuff:
1. Bot creates [Dependency Dashboard](https://github.com/xLEWKANx/renovatebot-test/issues/4) controlled by checkboxes 😮
2. It [can be configured](https://docs.renovatebot.com/key-concepts/scheduling/) to run at a specific time
3. It also can be configured for ruby and many more [other languages and package managers ](https://docs.renovatebot.com/modules/manager/)