# working example
- src/stories/index.stories.js
```
import React from 'react';
import { Button } from '@storybook/react/demo';

export default { title: 'Button' };

export const withText = () => <Button>Hello Button</Button>;

export const withEmoji = () => (
  <Button>
    <span role="img" aria-label="so cool">
      😀 😎 👍 💯
    </span>
  </Button>
);
```

# or
- 1-Button.stories.js
```
import React from 'react';
import { action } from '@storybook/addon-actions';
import { Button } from '@storybook/react/demo';

export default {
  title: 'Button',
  component: Button,
};

export const Text = () => <Button onClick={action('clicked')}>Hello Button</Button>;

export const Emoji = () => (
  <Button onClick={action('clicked')}>
    <span role="img" aria-label="so cool">
      😀 😎 👍 💯
    </span>
  </Button>
);
```

# the old storybook format - storiesof - (a lot of online documentation on this old format which adds confusion!)
- https://dev.to/ryanlanciaux/increase-your-productivity-with-storybook-s-new-component-story-format-531i
- https://storybook.js.org/docs/formats/storiesof-api/
- https://medium.com/storybookjs/component-story-format-66f4c32366df

# interesting to investigate - mdx - markdown mixed with jsx
- https://github.com/storybookjs/storybook/blob/next/addons/docs/docs/mdx.md
