Most of the time, we import our files using the following syntax :

```
import { stripeCreateToken } from '../../../src/utils/stripe';
```

Many problems with this syntax :
1) It's annoying to find where the "stripe.js" file is
2) Code is ugly
3) When you refactor and move your files, you have to change everywhere in your code

To solve this, in the utils folder, create a package.json file with the alias :
```
{
  "name": "utils"
}
```

Now, easily import the stripe file anywhere :
```
import { stripeCreateToken } from 'utils/stripe';
```
