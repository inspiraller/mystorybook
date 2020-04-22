# ref
- https://storybook.js.org/docs/guides/guide-react/

# after create react app
- https://storybook.js.org/docs/guides/guide-react/

# create react app
```
npx create-react-app mystorybook -- --use-npm
```

# cd into mystorbook and run this to generate files and dependencies
```
npx -p @storybook/cli sb init --type react_scripts
```

# create a new story

- 20-App.stories.js
```
import React from 'react';
import App from '../App';

export default {
  title: 'App',
  component: App,
};

export const ToStorybook = () => <App />;

ToStorybook.story = {
  name: 'to Storybook',
};

```
# run storybook
```
npm run storybook
```

done !!
