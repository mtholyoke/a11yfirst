# A11yFirst Plugins for CKEditor

This module adds the [A11yFirst CKEditor plugins](https://a11yfirst.library.illinois.edu/) to Drupal’s CKEditor.

### We are currently in process of moving this module to a new home: https://github.com/a11yfirst/drupal-plugin

**Note:** This is experimental, and not governed by A11yFirst. Use at your own risk.

Specifically, the source code of the plugins is copied from their [official distribution](https://github.com/a11yfirst/distribution) and included in this repo, since they are not otherwise independently available. This isn’t ideal, but it (mostly) works until someone comes up with a better plan.

## Installation

Before the move to the A11yFirst repo, you can `composer require mtholyoke/a11yfirst`. We will likely change the name after the move.

This module requires the [CKEditor FakeObjects](https://www.drupal.org/project/fakeobjects) module. While Composer will fetch its PHP code, the installation also requires getting that plugin’s JavaScript directly from https://ckeditor.com/cke4/addon/fakeobjects before it can be enabled.

## TODO

Drupal-specific documentation about what’s going on. Drupal likes to get its hooks all over CKEditor config, so a lot of things that are managed internally in the official distribution become external with this integration. This is also not ideal, but it’s far easier than replacing the editor entirely (which would have the same problems, but for all the other config also).

Heading button highlights but doesn’t show ✓ for selected level.

All button and dialog styles are different from [A11yFirst’s sample](https://a11yfirst.library.illinois.edu/demo/distribution/custom/a11yfirst.html).

Implement some tests, maybe?

Make this into a contrib module at drupal.org once we feel like enough of those things above are resolved.
